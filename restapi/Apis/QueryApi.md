# QueryApi

All URIs are relative to *http://localhost:8080/fitlayout-web*

Method | HTTP request | Description
------------- | ------------- | -------------
[**addQuery**](QueryApi.md#addQuery) | **POST** /api/r/{repoId}/query | Adds a saved a query
[**deleteQuery**](QueryApi.md#deleteQuery) | **DELETE** /api/r/{repoId}/query/{id} | Deletes a saved query
[**getQuery**](QueryApi.md#getQuery) | **GET** /api/r/{repoId}/query/{id} | Obtains a saved query
[**list**](QueryApi.md#list) | **GET** /api/r/{repoId}/query | Obtains all the saved queries


<a name="addQuery"></a>
# **addQuery**
> addQuery(repoId, SavedQueryDTO)

Adds a saved a query

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **repoId** | **String**| The ID of the artifact repository to use | [default to null]
 **SavedQueryDTO** | [**SavedQueryDTO**](../Models/SavedQueryDTO.md)|  | [optional]

### Return type

null (empty response body)

### Authorization

[jwt](../README.md#jwt)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: Not defined

<a name="deleteQuery"></a>
# **deleteQuery**
> deleteQuery(repoId, id)

Deletes a saved query

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **repoId** | **String**| The ID of the artifact repository to use | [default to null]
 **id** | **Long**|  | [default to null]

### Return type

null (empty response body)

### Authorization

[jwt](../README.md#jwt)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined

<a name="getQuery"></a>
# **getQuery**
> getQuery(repoId, id)

Obtains a saved query

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **repoId** | **String**| The ID of the artifact repository to use | [default to null]
 **id** | **Long**|  | [default to null]

### Return type

null (empty response body)

### Authorization

[jwt](../README.md#jwt)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined

<a name="list"></a>
# **list**
> list(repoId)

Obtains all the saved queries

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **repoId** | **String**| The ID of the artifact repository to use | [default to null]

### Return type

null (empty response body)

### Authorization

[jwt](../README.md#jwt)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined

