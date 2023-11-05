# RunServiceApi

All URIs are relative to *http://localhost:8080/fitlayout-web*

Method | HTTP request | Description
------------- | ------------- | -------------
[**renderJsonPage**](RunServiceApi.md#renderJsonPage) | **POST** /api/r/{repoId}/run/renderJson | Creates a new Page artifact from a JSON page description (e.g. obtained from a puppeteer backend or a client browser extension).


<a name="renderJsonPage"></a>
# **renderJsonPage**
> renderJsonPage(repoId, body)

Creates a new Page artifact from a JSON page description (e.g. obtained from a puppeteer backend or a client browser extension).

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **repoId** | **String**| The ID of the artifact repository to use | [default to null]
 **body** | **File**|  | [optional]

### Return type

null (empty response body)

### Authorization

[jwt](../README.md#jwt)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: Not defined

