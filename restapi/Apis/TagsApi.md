# TagsApi

All URIs are relative to *http://localhost:8080/fitlayout-web*

Method | HTTP request | Description
------------- | ------------- | -------------
[**getTags**](TagsApi.md#getTags) | **GET** /api/r/{repoId}/tags | Reads a list of tags defined in the repository


<a name="getTags"></a>
# **getTags**
> TagInfo getTags(repoId)

Reads a list of tags defined in the repository

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **repoId** | **String**| The ID of the artifact repository to use | [default to null]

### Return type

[**TagInfo**](../Models/TagInfo.md)

### Authorization

[jwt](../README.md#jwt)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

