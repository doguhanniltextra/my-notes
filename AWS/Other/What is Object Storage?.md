Unlike File Storage or Block Storage, Object Storage treats data as discrete units called _objects_. 
- Flat Hierarchy: Every object resides in a single, flat bucket. There are no true _folders_, only prefixes in the object's name.
- Components of an Object:
	- Data: The actual file (OHS, PDF report or an IoT log file)
	- Metadata: Customizable key-value pairs
	- Unique Identifier: The _Key_ used to retrieve the object.
- The S3 API: The Industry Standard, It is the universal language for object storage. Even if you don't use AWS, you will likely use S3 API to communicate with them.

|**Operation**|**Method**|**Description**|
|---|---|---|
|**PUT**|`PUT`|Uploads an object to a bucket.|
|**GET**|`GET`|Retrieves an object by its key.|
|**LIST**|`GET`|Returns a list of objects in a bucket (supports prefix filtering).|
|**DELETE**|`DELETE`|Removes an object.|
|**HEAD**|`HEAD`|Retrieves metadata without downloading the actual data.|
[[AWS]] 
