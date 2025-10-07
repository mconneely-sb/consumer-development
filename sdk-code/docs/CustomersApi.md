# IO.Swagger.Api.CustomersApi

All URIs are relative to *https://virtserver.swaggerhub.com/MConneely/OrderManagementAPI/1.0.0*

Method | HTTP request | Description
------------- | ------------- | -------------
[**CustomersGet**](CustomersApi.md#customersget) | **GET** /customers | 
[**CustomersIdGet**](CustomersApi.md#customersidget) | **GET** /customers/{id} | 

<a name="customersget"></a>
# **CustomersGet**
> List<Customer> CustomersGet ()



### Example
```csharp
using System;
using System.Diagnostics;
using IO.Swagger.Api;
using IO.Swagger.Client;
using IO.Swagger.Model;

namespace Example
{
    public class CustomersGetExample
    {
        public void main()
        {
            var apiInstance = new CustomersApi();

            try
            {
                List&lt;Customer&gt; result = apiInstance.CustomersGet();
                Debug.WriteLine(result);
            }
            catch (Exception e)
            {
                Debug.Print("Exception when calling CustomersApi.CustomersGet: " + e.Message );
            }
        }
    }
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**List<Customer>**](Customer.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: text/plain, application/json, text/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)
<a name="customersidget"></a>
# **CustomersIdGet**
> Customer CustomersIdGet (int? id)



### Example
```csharp
using System;
using System.Diagnostics;
using IO.Swagger.Api;
using IO.Swagger.Client;
using IO.Swagger.Model;

namespace Example
{
    public class CustomersIdGetExample
    {
        public void main()
        {
            var apiInstance = new CustomersApi();
            var id = 56;  // int? | 

            try
            {
                Customer result = apiInstance.CustomersIdGet(id);
                Debug.WriteLine(result);
            }
            catch (Exception e)
            {
                Debug.Print("Exception when calling CustomersApi.CustomersIdGet: " + e.Message );
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

[**Customer**](Customer.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: text/plain, application/json, text/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)
