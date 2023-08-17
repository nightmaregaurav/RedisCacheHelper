# RedisCacheHelper

RedisCacheHelper is a C# utility library that provides caching functionality using the StackExchange.Redis library without DI. It simplifies the process of storing and retrieving data from a Redis cache, allowing for efficient and reliable caching of objects.

## Features

- Simple and intuitive API for caching operations.
- Supports synchronous and asynchronous caching methods.
- Allows caching with optional expiration times.
- Provides synchronization of data retrieval using a provided function.

## Usage
1. Install the package from [NuGet](https://www.nuget.org/packages/nightmaregaurav.rediscachehelper).
2. Add these somewhere in your appsettings.json:
```json
     "Redis": {
          "Host": "your.redis.host",
          "Port": "PORT",
          "Password": "xxxxxxxxxx",
          "Prefix": "keyPrefix:"
     }
```
3. Use in code
```csharp
// Example usage of RedisCacheHelper
using RedisCacheHelper;
// Rest of the codes...
//
CacheHelper.Set("myKey", myObject);
var cachedObject = CacheHelper.Get<MyType>("myKey");
//
// Rest of the codes...
```

## License

RedisCacheHelper is released under the MIT License. You can find the full license details in the [LICENSE](LICENSE) file.

Made with ❤️ by [NightmareGaurav](https://github.com/nightmaregaurav).

---
Open For Contribution
---
We welcome contributions from the community! If you find any issues or have suggestions for improvements, feel free to open a pull request or issue. Your contributions help make this project better for everyone.
