# IO.Swagger.Api.OrdersApi

All URIs are relative to *https://virtserver.swaggerhub.com/MConneely/OrderManagementAPI/1.0.0*

Method | HTTP request | Description
------------- | ------------- | -------------
[**ApiOrdersGet**](OrdersApi.md#apiordersget) | **GET** /api/orders | 
[**ApiOrdersIdDelete**](OrdersApi.md#apiordersiddelete) | **DELETE** /api/orders/{id} | 
[**ApiOrdersIdGet**](OrdersApi.md#apiordersidget) | **GET** /api/orders/{id} | 
[**ApiOrdersIdPut**](OrdersApi.md#apiordersidput) | **PUT** /api/orders/{id} | 
[**ApiOrdersIdStatusPatch**](OrdersApi.md#apiordersidstatuspatch) | **PATCH** /api/orders/{id}/status | 
[**ApiOrdersPost**](OrdersApi.md#apiorderspost) | **POST** /api/orders | 
[**ApiOrdersStatusStatusGet**](OrdersApi.md#apiordersstatusstatusget) | **GET** /api/orders/status/{status} | 

<a name="apiordersget"></a>
# **ApiOrdersGet**
> List<OrderDto> ApiOrdersGet ()



### Example
```csharp
using System;
using System.Diagnostics;
using IO.Swagger.Api;
using IO.Swagger.Client;
using IO.Swagger.Model;

namespace Example
{
    public class ApiOrdersGetExample
    {
        public void main()
        {
            var apiInstance = new OrdersApi();

            try
            {
                List&lt;OrderDto&gt; result = apiInstance.ApiOrdersGet();
                Debug.WriteLine(result);
            }
            catch (Exception e)
            {
                Debug.Print("Exception when calling OrdersApi.ApiOrdersGet: " + e.Message );
            }
        }
    }
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**List<OrderDto>**](OrderDto.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: text/plain, application/json, text/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)
<a name="apiordersiddelete"></a>
# **ApiOrdersIdDelete**
> void ApiOrdersIdDelete (int? id)



### Example
```csharp
using System;
using System.Diagnostics;
using IO.Swagger.Api;
using IO.Swagger.Client;
using IO.Swagger.Model;

namespace Example
{
    public class ApiOrdersIdDeleteExample
    {
        public void main()
        {
            var apiInstance = new OrdersApi();
            var id = 56;  // int? | 

            try
            {
                apiInstance.ApiOrdersIdDelete(id);
            }
            catch (Exception e)
            {
                Debug.Print("Exception when calling OrdersApi.ApiOrdersIdDelete: " + e.Message );
            }
        }
    }
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int?**|  | 

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)
<a name="apiordersidget"></a>
# **ApiOrdersIdGet**
> OrderDto ApiOrdersIdGet (int? id)



### Example
```csharp
using System;
using System.Diagnostics;
using IO.Swagger.Api;
using IO.Swagger.Client;
using IO.Swagger.Model;

namespace Example
{
    public class ApiOrdersIdGetExample
    {
        public void main()
        {
            var apiInstance = new OrdersApi();
            var id = 56;  // int? | 

            try
            {
                OrderDto result = apiInstance.ApiOrdersIdGet(id);
                Debug.WriteLine(result);
            }
            catch (Exception e)
            {
                Debug.Print("Exception when calling OrdersApi.ApiOrdersIdGet: " + e.Message );
            }
        }
    }
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int?**|  | 

### Return type

[**OrderDto**](OrderDto.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: text/plain, application/json, text/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)
<a name="apiordersidput"></a>
# **ApiOrdersIdPut**
> OrderDto ApiOrdersIdPut (int? id, UpdateOrderDto body = null)



### Example
```csharp
using System;
using System.Diagnostics;
using IO.Swagger.Api;
using IO.Swagger.Client;
using IO.Swagger.Model;

namespace Example
{
    public class ApiOrdersIdPutExample
    {
        public void main()
        {
            var apiInstance = new OrdersApi();
            var id = 56;  // int? | 
            var body = new UpdateOrderDto(); // UpdateOrderDto |  (optional) 

            try
            {
                OrderDto result = apiInstance.ApiOrdersIdPut(id, body);
                Debug.WriteLine(result);
            }
            catch (Exception e)
            {
                Debug.Print("Exception when calling OrdersApi.ApiOrdersIdPut: " + e.Message );
            }
        }
    }
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int?**|  | 
 **body** | [**UpdateOrderDto**](UpdateOrderDto.md)|  | [optional] 

### Return type

[**OrderDto**](OrderDto.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json, text/json, application/_*+json
 - **Accept**: text/plain, application/json, text/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)
<a name="apiordersidstatuspatch"></a>
# **ApiOrdersIdStatusPatch**
> OrderDto ApiOrdersIdStatusPatch (int? id, UpdateOrderStatusDto body = null)



### Example
```csharp
using System;
using System.Diagnostics;
using IO.Swagger.Api;
using IO.Swagger.Client;
using IO.Swagger.Model;

namespace Example
{
    public class ApiOrdersIdStatusPatchExample
    {
        public void main()
        {
            var apiInstance = new OrdersApi();
            var id = 56;  // int? | 
            var body = new UpdateOrderStatusDto(); // UpdateOrderStatusDto |  (optional) 

            try
            {
                OrderDto result = apiInstance.ApiOrdersIdStatusPatch(id, body);
                Debug.WriteLine(result);
            }
            catch (Exception e)
            {
                Debug.Print("Exception when calling OrdersApi.ApiOrdersIdStatusPatch: " + e.Message );
            }
        }
    }
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int?**|  | 
 **body** | [**UpdateOrderStatusDto**](UpdateOrderStatusDto.md)|  | [optional] 

### Return type

[**OrderDto**](OrderDto.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json, text/json, application/_*+json
 - **Accept**: text/plain, application/json, text/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)
<a name="apiorderspost"></a>
# **ApiOrdersPost**
> OrderDto ApiOrdersPost (CreateOrderDto body = null)



### Example
```csharp
using System;
using System.Diagnostics;
using IO.Swagger.Api;
using IO.Swagger.Client;
using IO.Swagger.Model;

namespace Example
{
    public class ApiOrdersPostExample
    {
        public void main()
        {
            var apiInstance = new OrdersApi();
            var body = new CreateOrderDto(); // CreateOrderDto |  (optional) 

            try
            {
                OrderDto result = apiInstance.ApiOrdersPost(body);
                Debug.WriteLine(result);
            }
            catch (Exception e)
            {
                Debug.Print("Exception when calling OrdersApi.ApiOrdersPost: " + e.Message );
            }
        }
    }
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**CreateOrderDto**](CreateOrderDto.md)|  | [optional] 

### Return type

[**OrderDto**](OrderDto.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json, text/json, application/_*+json
 - **Accept**: text/plain, application/json, text/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)
<a name="apiordersstatusstatusget"></a>
# **ApiOrdersStatusStatusGet**
> List<OrderDto> ApiOrdersStatusStatusGet (string status)



### Example
```csharp
using System;
using System.Diagnostics;
using IO.Swagger.Api;
using IO.Swagger.Client;
using IO.Swagger.Model;

namespace Example
{
    public class ApiOrdersStatusStatusGetExample
    {
        public void main()
        {
            var apiInstance = new OrdersApi();
            var status = status_example;  // string | 

            try
            {
                List&lt;OrderDto&gt; result = apiInstance.ApiOrdersStatusStatusGet(status);
                Debug.WriteLine(result);
            }
            catch (Exception e)
            {
                Debug.Print("Exception when calling OrdersApi.ApiOrdersStatusStatusGet: " + e.Message );
            }
        }
    }
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **status** | **string**|  | 

### Return type

[**List<OrderDto>**](OrderDto.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: text/plain, application/json, text/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)
