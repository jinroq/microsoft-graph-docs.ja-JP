---
title: リスト privilegedRoleAssignments
description: 組織のすべての役割の割り当てに対応する privilegedRoleAssignment オブジェクトの一覧を取得します。
localization_priority: Normal
ms.openlocfilehash: c576e0d9c0a278e02159e02cea94ddd927561e08
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32538623"
---
# <a name="list-privilegedroleassignments"></a><span data-ttu-id="a3858-103">リスト privilegedRoleAssignments</span><span class="sxs-lookup"><span data-stu-id="a3858-103">List privilegedRoleAssignments</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a3858-104">組織のすべての役割の割り当てに対応する[privilegedRoleAssignment](../resources/privilegedroleassignment.md)オブジェクトの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="a3858-104">Retrieve a list of [privilegedRoleAssignment](../resources/privilegedroleassignment.md) objects, which correspond to all role assignments for the organization.</span></span>
## <a name="permissions"></a><span data-ttu-id="a3858-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="a3858-105">Permissions</span></span>
<span data-ttu-id="a3858-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a3858-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="a3858-108">リクエスターは、_特権の役割管理者_、_全体管理_者、_セキュリティ管理者_、または_セキュリティ閲覧_者のいずれかの役割を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="a3858-108">The requestor needs to have one of the following roles: _Privileged Role Administrator_, _Global Administrator_, _Security Administrator_, or _Security Reader_.</span></span> 

|<span data-ttu-id="a3858-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a3858-109">Permission type</span></span>      | <span data-ttu-id="a3858-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="a3858-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a3858-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a3858-111">Delegated (work or school account)</span></span> | <span data-ttu-id="a3858-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a3858-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a3858-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a3858-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a3858-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a3858-114">Not supported.</span></span>    |
|<span data-ttu-id="a3858-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a3858-115">Application</span></span> | <span data-ttu-id="a3858-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a3858-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a3858-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a3858-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoleAssignments
```
## <a name="optional-query-parameters"></a><span data-ttu-id="a3858-118">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="a3858-118">Optional query parameters</span></span>
<span data-ttu-id="a3858-119">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="a3858-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a3858-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a3858-120">Request headers</span></span>
| <span data-ttu-id="a3858-121">名前</span><span class="sxs-lookup"><span data-stu-id="a3858-121">Name</span></span>      |<span data-ttu-id="a3858-122">説明</span><span class="sxs-lookup"><span data-stu-id="a3858-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a3858-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a3858-123">Authorization</span></span>  | <span data-ttu-id="a3858-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="a3858-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a3858-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="a3858-126">Request body</span></span>
<span data-ttu-id="a3858-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="a3858-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a3858-128">応答</span><span class="sxs-lookup"><span data-stu-id="a3858-128">Response</span></span>

<span data-ttu-id="a3858-129">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[privilegedRoleAssignment](../resources/privilegedroleassignment.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="a3858-129">If successful, this method returns a `200 OK` response code and collection of [privilegedRoleAssignment](../resources/privilegedroleassignment.md) objects in the response body.</span></span>

<span data-ttu-id="a3858-130">テナントが PIM に登録されている必要があることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="a3858-130">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="a3858-131">それ以外の場合、HTTP 403 の禁止状態コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="a3858-131">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="examples"></a><span data-ttu-id="a3858-132">例</span><span class="sxs-lookup"><span data-stu-id="a3858-132">Examples</span></span>
### <a name="get-all-role-assignments"></a><span data-ttu-id="a3858-133">すべての役割の割り当てを取得する</span><span class="sxs-lookup"><span data-stu-id="a3858-133">Get all role assignments</span></span>
##### <a name="request"></a><span data-ttu-id="a3858-134">要求</span><span class="sxs-lookup"><span data-stu-id="a3858-134">Request</span></span>
<span data-ttu-id="a3858-135">次の例は、すべての役割の割り当てを取得するための要求を示しています。</span><span class="sxs-lookup"><span data-stu-id="a3858-135">The following example shows a request to get all role assignments:</span></span>
<!-- {
  "blockType": "request",
  "name": "get_privilegedroleassignments"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoleAssignments
```
##### <a name="response"></a><span data-ttu-id="a3858-136">応答</span><span class="sxs-lookup"><span data-stu-id="a3858-136">Response</span></span>
<span data-ttu-id="a3858-137">次の例は応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="a3858-137">The following example shows the response.</span></span> <span data-ttu-id="a3858-138">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="a3858-138">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="a3858-139">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="a3858-139">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedRoleAssignment",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 237

{
  "value": [
    {
      "id": "id-value",
      "userId": "userId-value",
      "roleId": "roleId-value",
      "isElevated": true,
      "expirationDateTime": "2016-10-19T10:37:00Z",
      "resultMessage": "resultMessage-value"
    }
  ]
}
```
### <a name="get-active-role-assignments"></a><span data-ttu-id="a3858-140">アクティブな役割の割り当てを取得する</span><span class="sxs-lookup"><span data-stu-id="a3858-140">Get active role assignments</span></span>
##### <a name="request"></a><span data-ttu-id="a3858-141">要求</span><span class="sxs-lookup"><span data-stu-id="a3858-141">Request</span></span> 
<span data-ttu-id="a3858-142">次の例は、アクティブな役割の割り当てを照会する要求を示しています。</span><span class="sxs-lookup"><span data-stu-id="a3858-142">The following example shows a request to query active role assignments:</span></span>
<!-- {
  "blockType": "request",
  "name": "get_privilegedroleassignments"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoleAssignments?$filter=isElevated%20eq%20true
```
##### <a name="response"></a><span data-ttu-id="a3858-143">応答</span><span class="sxs-lookup"><span data-stu-id="a3858-143">Response</span></span>
<span data-ttu-id="a3858-144">次の例は応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="a3858-144">The following example shows the response.</span></span> <span data-ttu-id="a3858-145">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="a3858-145">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="a3858-146">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="a3858-146">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedRoleAssignment",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 237

{
  "value": [
        {
            "id": "0f693614-c255-4cf5-92fa-74e770c656d8_62e90394-69f5-4237-9190-012177145e10",
            "userId": "0f693614-c255-4cf5-92fa-74e770c656d8",
            "roleId": "62e90394-69f5-4237-9190-012177145e10",
            "isElevated": true,
            "expirationDateTime": null,
            "resultMessage": null
        },
        {
            "id": "0f693614-c255-4cf5-92fa-74e770c656d8_95e79109-95c0-4d8e-aee3-d01accf2d47b",
            "userId": "0f693614-c255-4cf5-92fa-74e770c656d8",
            "roleId": "95e79109-95c0-4d8e-aee3-d01accf2d47b",
            "isElevated": true,
            "expirationDateTime": "2017-07-25T17:38:49.563Z",
            "resultMessage": null
        }
  ]
}
```
### <a name="get-permanent-role-assignments"></a><span data-ttu-id="a3858-147">永続的な役割の割り当てを取得する</span><span class="sxs-lookup"><span data-stu-id="a3858-147">Get permanent role assignments</span></span>
##### <a name="request"></a><span data-ttu-id="a3858-148">要求</span><span class="sxs-lookup"><span data-stu-id="a3858-148">Request</span></span> 
<span data-ttu-id="a3858-149">次の例は、永続的な役割の割り当てを照会する``expirationDateTime``要求を``null``示しています。 value は次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="a3858-149">The following example shows a request to query permanent role assignments, where ``expirationDateTime`` value is ``null``:</span></span>
<!-- {
  "blockType": "request",
  "name": "get_privilegedroleassignments"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoleAssignments?$filter=isElevated%20eq%20true%20and%20expirationDateTime%20eq%20null
```
##### <a name="response"></a><span data-ttu-id="a3858-150">応答</span><span class="sxs-lookup"><span data-stu-id="a3858-150">Response</span></span>
<span data-ttu-id="a3858-151">次の例は応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="a3858-151">The following example shows the response.</span></span> <span data-ttu-id="a3858-152">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="a3858-152">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="a3858-153">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="a3858-153">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedRoleAssignment",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 237

{
  "value": [
        {
            "id": "0f693614-c255-4cf5-92fa-74e770c656d8_194ae4cb-b126-40b2-bd5b-6091b380977d",
            "userId": "0f693614-c255-4cf5-92fa-74e770c656d8",
            "roleId": "194ae4cb-b126-40b2-bd5b-6091b380977d",
            "isElevated": true,
            "expirationDateTime": null,
            "resultMessage": null
        },
        {
            "id": "0f693614-c255-4cf5-92fa-74e770c656d8_44367163-eba1-44c3-98af-f5787879f96a",
            "userId": "0f693614-c255-4cf5-92fa-74e770c656d8",
            "roleId": "44367163-eba1-44c3-98af-f5787879f96a",
            "isElevated": true,
            "expirationDateTime": null,
            "resultMessage": null
        }
  ]
}
```
### <a name="get-eligible-role-assignments"></a><span data-ttu-id="a3858-154">対象の役割の割り当てを取得する</span><span class="sxs-lookup"><span data-stu-id="a3858-154">Get eligible role assignments</span></span>
##### <a name="request"></a><span data-ttu-id="a3858-155">要求</span><span class="sxs-lookup"><span data-stu-id="a3858-155">Request</span></span> 
<span data-ttu-id="a3858-156">次の例は、アクティブなものとアクティブでないものを含む、対象となる役割の割り当てを照会する要求を示しています。</span><span class="sxs-lookup"><span data-stu-id="a3858-156">The following example shows a request to query eligible role assignments, including the active and non-active ones:</span></span>
<!-- {
  "blockType": "request",
  "name": "get_privilegedroleassignments"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoleAssignments?$filter=isElevated%20eq%20true%20and%20expirationDateTime%20ne%20null%20or%20isElevated%20eq%20false
```
##### <a name="response"></a><span data-ttu-id="a3858-157">応答</span><span class="sxs-lookup"><span data-stu-id="a3858-157">Response</span></span> 
<span data-ttu-id="a3858-158">次の例は応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="a3858-158">The following example shows the response.</span></span> <span data-ttu-id="a3858-159">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="a3858-159">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="a3858-160">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="a3858-160">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedRoleAssignment",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 237

{
  "value": [
        {
            "id": "0f693614-c255-4cf5-92fa-74e770c656d8_95e79109-95c0-4d8e-aee3-d01accf2d47b",
            "userId": "0f693614-c255-4cf5-92fa-74e770c656d8",
            "roleId": "95e79109-95c0-4d8e-aee3-d01accf2d47b",
            "isElevated": true,
            "expirationDateTime": "2017-07-25T18:42:26.823Z",
            "resultMessage": null
        },
        {
            "id": "2cf9eef8-bc67-4aa4-bb65-75cc9e5c3f81_194ae4cb-b126-40b2-bd5b-6091b380977d",
            "userId": "2cf9eef8-bc67-4aa4-bb65-75cc9e5c3f81",
            "roleId": "194ae4cb-b126-40b2-bd5b-6091b380977d",
            "isElevated": false,
            "expirationDateTime": null,
            "resultMessage": null
        },
        {
            "id": "2cf9eef8-bc67-4aa4-bb65-75cc9e5c3f81_9360feb5-f418-4baa-8175-e2a00bac4301",
            "userId": "2cf9eef8-bc67-4aa4-bb65-75cc9e5c3f81",
            "roleId": "9360feb5-f418-4baa-8175-e2a00bac4301",
            "isElevated": false,
            "expirationDateTime": null,
            "resultMessage": null
        },
        {
            "id": "2cf9eef8-bc67-4aa4-bb65-75cc9e5c3f81_95e79109-95c0-4d8e-aee3-d01accf2d47b",
            "userId": "2cf9eef8-bc67-4aa4-bb65-75cc9e5c3f81",
            "roleId": "95e79109-95c0-4d8e-aee3-d01accf2d47b",
            "isElevated": false,
            "expirationDateTime": null,
            "resultMessage": null
        }
  ]
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List privilegedRoleAssignments",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/privilegedroleassignment-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
