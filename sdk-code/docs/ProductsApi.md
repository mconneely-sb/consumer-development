# IO.Swagger.Api.ProductsApi

All URIs are relative to *https://virtserver.swaggerhub.com/MConneely/OrderManagementAPI/1.0.0*

Method | HTTP request | Description
------------- | ------------- | -------------
[**ProductsGet**](ProductsApi.md#productsget) | **GET** /products | 
[**ProductsIdGet**](ProductsApi.md#productsidget) | **GET** /products/{id} | 

<a name="productsget"></a>
# **ProductsGet**
> List<Product> ProductsGet ()



### Example
```csharp
using System;
using System.Diagnostics;
using IO.Swagger.Api;
using IO.Swagger.Client;
using IO.Swagger.Model;

namespace Example
{
    public class ProductsGetExample
    {
        public void main()
        {
            var apiInstance = new ProductsApi();

            try
            {
                List&lt;Product&gt; result = apiInstance.ProductsGet();
                Debug.WriteLine(result);
            }
            catch (Exception e)
            {
                Debug.Print("Exception when calling ProductsApi.ProductsGet: " + e.Message );
            }
        }
    }
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**List<Product>**](Product.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: text/plain, application/json, text/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)
<a name="productsidget"></a>
# **ProductsIdGet**
> Product ProductsIdGet (int? id)



### Example
```csharp
using System;
using System.Diagnostics;
using IO.Swagger.Api;
using IO.Swagger.Client;
using IO.Swagger.Model;

namespace Example
{
    public class ProductsIdGetExample
    {
        public void main()
        {
            var apiInstance = new ProductsApi();
            var id = 56;  // int? | 

            try
            {
                Product result = apiInstance.ProductsIdGet(id);
                Debug.WriteLine(result);
            }
            catch (Exception e)
            {
                Debug.Print("Exception when calling ProductsApi.ProductsIdGet: " + e.Message );
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

[**Product**](Product.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: text/plain, application/json, text/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)
