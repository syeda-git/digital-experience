# ResourceInfo class

The ResourceInfo class is a wrapper class for a resource id and collection name tuple.

```
public class com.ibm.wcp.analysis.event.ResourceInfo extends Object
                                                     implements Serializable
```

Get an overview of the methods of the ResourceInfo class.

|Method|Explanation|
|------|-----------|
|public ResourceInfo( String resourceId,<br>                     String collectionName )|Constructor.|
|public ResourceInfo( )|Constructor.|
|public String getResourceId( )|Returns the id of the resource.|
|public void setResourceId( String resourceId )|Sets the id of the resource.|
|public String getCollectionName( )|Returns the name of the collection that contains this resource.|
|public void setCollectionName( String collectionName )|Sets the name of the collection that contains this resource.|
|public String toString( )|Returns a String representation of this resource tuple.|
|public boolean equals( ResourceInfo resourceInfo )|Returns true if and only if \(1\) the objects are the same or \(2\) the resource id and collection name information is equal.|
|public int hashCode( )|Returns a hash code enabling objects of this type to be used as hash keys.|


