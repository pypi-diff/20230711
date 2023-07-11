# Comparing `tmp/atro_victoria-0.0.2.tar.gz` & `tmp/atro_victoria-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atro_victoria-0.0.2.tar", max compression
+gzip compressed data, was "atro_victoria-0.0.3.tar", max compression
```

## Comparing `atro_victoria-0.0.2.tar` & `atro_victoria-0.0.3.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0        0 2023-07-09 16:47:06.656790 atro_victoria-0.0.2/README.md
--rw-r--r--   0        0        0     1723 2023-07-09 17:54:53.428384 atro_victoria-0.0.2/atro_victoria/__init__.py
--rw-r--r--   0        0        0      409 2023-07-09 17:54:45.411547 atro_victoria-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      450 1970-01-01 00:00:00.000000 atro_victoria-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-09 16:47:06.656790 atro_victoria-0.0.3/README.md
+-rw-r--r--   0        0        0     1720 2023-07-11 20:21:24.548272 atro_victoria-0.0.3/atro_victoria/__init__.py
+-rw-r--r--   0        0        0      409 2023-07-11 20:21:35.185160 atro_victoria-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      450 1970-01-01 00:00:00.000000 atro_victoria-0.0.3/PKG-INFO
```

### Comparing `atro_victoria-0.0.2/atro_victoria/__init__.py` & `atro_victoria-0.0.3/atro_victoria/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 def strigify_datetime(dt: datetime):
   return int(dt.timestamp() * 1000)
 
 class VmCsvRowBase(BaseSettings):
   job: str 
   name: str
-  timestamp: PastDatetime = datetime.utcnow()
+  timestamp: PastDatetime = datetime.now()
   url: AnyHttpUrl = Url("http://localhost:8480/")
   model_config = SettingsConfigDict(env_prefix='ATRO_VM_', env_file=[(Path.home() / ".config" / "atro" / "vm.env").as_posix(), ".env"]
 )
     
   def format(self):
     vals = self.model_dump()
     counter = 0
```

