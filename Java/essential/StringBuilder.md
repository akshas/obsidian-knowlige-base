``` java
StringBuilder stringBuilder = new StringBuilder();
```

**Or**

```java
StringBuilder stringBuilder = new StringBuilder("string");
```
___


## Append
```java
	stringBuilder.append("one");
	stringBuilder.append(2);
	stringBuilder.append(false);
	stringBuilder.append(null);
	
	```
***returns "one2falsenull"***
___


## Insert
```java
	stringBUilder.insert(0, "A")

```
***returns "Aone2falsenull"***
___


## Delete

```java
stringBUilder.delete(int sart, int end);
```