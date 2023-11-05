# ServiceApi

All URIs are relative to *http://localhost:8080/fitlayout-web*

Method | HTTP request | Description
------------- | ------------- | -------------
[**getServiceConfig**](ServiceApi.md#getServiceConfig) | **GET** /api/service/config | Gets the default configuration of an artifact service.
[**getServiceList**](ServiceApi.md#getServiceList) | **GET** /api/service | Gets a list of available artifact services.
[**invoke**](ServiceApi.md#invoke) | **POST** /api/service | Invokes a service and returns the resulting artifact
[**listOperators**](ServiceApi.md#listOperators) | **GET** /api/operator | Gets a list of available area tree operator services.
[**ping**](ServiceApi.md#ping) | **GET** /api/service/ping | Returns &#39;ok&#39;.


<a name="getServiceConfig"></a>
# **getServiceConfig**
> ServiceParams getServiceConfig(id)

Gets the default configuration of an artifact service.

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **String**|  | [optional] [default to null]

### Return type

[**ServiceParams**](../Models/ServiceParams.md)

### Authorization

[jwt](../README.md#jwt)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="getServiceList"></a>
# **getServiceList**
> List getServiceList()

Gets a list of available artifact services.

### Parameters
This endpoint does not need any parameter.

### Return type

[**List**](../Models/ArtifactServiceDescr.md)

### Authorization

[jwt](../README.md#jwt)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="invoke"></a>
# **invoke**
> invoke(ServiceParams)

Invokes a service and returns the resulting artifact

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ServiceParams** | [**ServiceParams**](../Models/ServiceParams.md)|  | [optional]

### Return type

null (empty response body)

### Authorization

[jwt](../README.md#jwt)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: Not defined

<a name="listOperators"></a>
# **listOperators**
> List listOperators()

Gets a list of available area tree operator services.

### Parameters
This endpoint does not need any parameter.

### Return type

[**List**](../Models/ParametrizedServiceDescr.md)

### Authorization

[jwt](../README.md#jwt)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="ping"></a>
# **ping**
> String ping()

Returns &#39;ok&#39;.

### Parameters
This endpoint does not need any parameter.

### Return type

[**String**](../Models/string.md)

### Authorization

[jwt](../README.md#jwt)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: */*

