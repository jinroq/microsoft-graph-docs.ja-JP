---
title: リスト privilegedRoleAssignments
description: 組織のすべての役割の割り当てに対応する privilegedRoleAssignment オブジェクトの一覧を取得します。
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 4a55d33bf6c9bcecc8a1c643176a630648f7e379
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35983388"
---
# <a name="list-privilegedroleassignments"></a><span data-ttu-id="f52c7-103">リスト privilegedRoleAssignments</span><span class="sxs-lookup"><span data-stu-id="f52c7-103">List privilegedRoleAssignments</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f52c7-104">組織のすべての役割の割り当てに対応する[privilegedRoleAssignment](../resources/privilegedroleassignment.md)オブジェクトの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="f52c7-104">Retrieve a list of [privilegedRoleAssignment](../resources/privilegedroleassignment.md) objects, which correspond to all role assignments for the organization.</span></span>
## <a name="permissions"></a><span data-ttu-id="f52c7-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f52c7-105">Permissions</span></span>
<span data-ttu-id="f52c7-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f52c7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="f52c7-108">リクエスターは、_特権の役割管理者_、_全体管理_者、_セキュリティ管理者_、または_セキュリティ閲覧_者のいずれかの役割を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="f52c7-108">The requestor needs to have one of the following roles: _Privileged Role Administrator_, _Global Administrator_, _Security Administrator_, or _Security Reader_.</span></span> 

|<span data-ttu-id="f52c7-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f52c7-109">Permission type</span></span>      | <span data-ttu-id="f52c7-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="f52c7-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f52c7-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f52c7-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f52c7-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f52c7-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="f52c7-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f52c7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f52c7-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f52c7-114">Not supported.</span></span>    |
|<span data-ttu-id="f52c7-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f52c7-115">Application</span></span> | <span data-ttu-id="f52c7-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f52c7-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f52c7-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f52c7-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoleAssignments
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f52c7-118">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="f52c7-118">Optional query parameters</span></span>
<span data-ttu-id="f52c7-119">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="f52c7-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f52c7-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f52c7-120">Request headers</span></span>
| <span data-ttu-id="f52c7-121">名前</span><span class="sxs-lookup"><span data-stu-id="f52c7-121">Name</span></span>      |<span data-ttu-id="f52c7-122">説明</span><span class="sxs-lookup"><span data-stu-id="f52c7-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f52c7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f52c7-123">Authorization</span></span>  | <span data-ttu-id="f52c7-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="f52c7-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f52c7-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="f52c7-126">Request body</span></span>
<span data-ttu-id="f52c7-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="f52c7-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f52c7-128">応答</span><span class="sxs-lookup"><span data-stu-id="f52c7-128">Response</span></span>

<span data-ttu-id="f52c7-129">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[privilegedRoleAssignment](../resources/privilegedroleassignment.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="f52c7-129">If successful, this method returns a `200 OK` response code and collection of [privilegedRoleAssignment](../resources/privilegedroleassignment.md) objects in the response body.</span></span>

<span data-ttu-id="f52c7-130">テナントが PIM に登録されている必要があることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="f52c7-130">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="f52c7-131">それ以外の場合、HTTP 403 の禁止状態コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="f52c7-131">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="examples"></a><span data-ttu-id="f52c7-132">例</span><span class="sxs-lookup"><span data-stu-id="f52c7-132">Examples</span></span>
### <a name="get-all-role-assignments"></a><span data-ttu-id="f52c7-133">すべての役割の割り当てを取得する</span><span class="sxs-lookup"><span data-stu-id="f52c7-133">Get all role assignments</span></span>
##### <a name="request"></a><span data-ttu-id="f52c7-134">要求</span><span class="sxs-lookup"><span data-stu-id="f52c7-134">Request</span></span>
<span data-ttu-id="f52c7-135">次の例は、すべての役割の割り当てを取得するための要求を示しています。</span><span class="sxs-lookup"><span data-stu-id="f52c7-135">The following example shows a request to get all role assignments:</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="f52c7-136">プロトコル</span><span class="sxs-lookup"><span data-stu-id="f52c7-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_privilegedroleassignments"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoleAssignments
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="f52c7-137">C#</span><span class="sxs-lookup"><span data-stu-id="f52c7-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-privilegedroleassignments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f52c7-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="f52c7-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-privilegedroleassignments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f52c7-139">目的-C</span><span class="sxs-lookup"><span data-stu-id="f52c7-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-privilegedroleassignments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="f52c7-140">Java</span><span class="sxs-lookup"><span data-stu-id="f52c7-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-privilegedroleassignments-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="f52c7-141">応答</span><span class="sxs-lookup"><span data-stu-id="f52c7-141">Response</span></span>
<span data-ttu-id="f52c7-142">次の例は応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="f52c7-142">The following example shows the response.</span></span> <span data-ttu-id="f52c7-143">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="f52c7-143">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="f52c7-144">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="f52c7-144">All of the properties will be returned from an actual call.</span></span>
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
### <a name="get-active-role-assignments"></a><span data-ttu-id="f52c7-145">アクティブな役割の割り当てを取得する</span><span class="sxs-lookup"><span data-stu-id="f52c7-145">Get active role assignments</span></span>
##### <a name="request"></a><span data-ttu-id="f52c7-146">要求</span><span class="sxs-lookup"><span data-stu-id="f52c7-146">Request</span></span> 
<span data-ttu-id="f52c7-147">次の例は、アクティブな役割の割り当てを照会する要求を示しています。</span><span class="sxs-lookup"><span data-stu-id="f52c7-147">The following example shows a request to query active role assignments:</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="f52c7-148">プロトコル</span><span class="sxs-lookup"><span data-stu-id="f52c7-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_privilegedroleassignments"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoleAssignments?$filter=isElevated%20eq%20true
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="f52c7-149">C#</span><span class="sxs-lookup"><span data-stu-id="f52c7-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-privilegedroleassignments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f52c7-150">Javascript</span><span class="sxs-lookup"><span data-stu-id="f52c7-150">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-privilegedroleassignments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f52c7-151">目的-C</span><span class="sxs-lookup"><span data-stu-id="f52c7-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-privilegedroleassignments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="f52c7-152">Java</span><span class="sxs-lookup"><span data-stu-id="f52c7-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-privilegedroleassignments-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="f52c7-153">応答</span><span class="sxs-lookup"><span data-stu-id="f52c7-153">Response</span></span>
<span data-ttu-id="f52c7-154">次の例は応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="f52c7-154">The following example shows the response.</span></span> <span data-ttu-id="f52c7-155">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="f52c7-155">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="f52c7-156">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="f52c7-156">All of the properties will be returned from an actual call.</span></span>
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
### <a name="get-permanent-role-assignments"></a><span data-ttu-id="f52c7-157">永続的な役割の割り当てを取得する</span><span class="sxs-lookup"><span data-stu-id="f52c7-157">Get permanent role assignments</span></span>
##### <a name="request"></a><span data-ttu-id="f52c7-158">要求</span><span class="sxs-lookup"><span data-stu-id="f52c7-158">Request</span></span> 
<span data-ttu-id="f52c7-159">次の例は、永続的な役割の割り当てを照会する``expirationDateTime``要求を``null``示しています。 value は次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="f52c7-159">The following example shows a request to query permanent role assignments, where ``expirationDateTime`` value is ``null``:</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="f52c7-160">プロトコル</span><span class="sxs-lookup"><span data-stu-id="f52c7-160">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_privilegedroleassignments"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoleAssignments?$filter=isElevated%20eq%20true%20and%20expirationDateTime%20eq%20null
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="f52c7-161">C#</span><span class="sxs-lookup"><span data-stu-id="f52c7-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-privilegedroleassignments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f52c7-162">Javascript</span><span class="sxs-lookup"><span data-stu-id="f52c7-162">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-privilegedroleassignments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f52c7-163">目的-C</span><span class="sxs-lookup"><span data-stu-id="f52c7-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-privilegedroleassignments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="f52c7-164">Java</span><span class="sxs-lookup"><span data-stu-id="f52c7-164">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-privilegedroleassignments-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="f52c7-165">応答</span><span class="sxs-lookup"><span data-stu-id="f52c7-165">Response</span></span>
<span data-ttu-id="f52c7-166">次の例は応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="f52c7-166">The following example shows the response.</span></span> <span data-ttu-id="f52c7-167">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="f52c7-167">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="f52c7-168">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="f52c7-168">All of the properties will be returned from an actual call.</span></span>
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
### <a name="get-eligible-role-assignments"></a><span data-ttu-id="f52c7-169">対象の役割の割り当てを取得する</span><span class="sxs-lookup"><span data-stu-id="f52c7-169">Get eligible role assignments</span></span>
##### <a name="request"></a><span data-ttu-id="f52c7-170">要求</span><span class="sxs-lookup"><span data-stu-id="f52c7-170">Request</span></span> 
<span data-ttu-id="f52c7-171">次の例は、アクティブなものとアクティブでないものを含む、対象となる役割の割り当てを照会する要求を示しています。</span><span class="sxs-lookup"><span data-stu-id="f52c7-171">The following example shows a request to query eligible role assignments, including the active and non-active ones:</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="f52c7-172">プロトコル</span><span class="sxs-lookup"><span data-stu-id="f52c7-172">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_privilegedroleassignments"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoleAssignments?$filter=isElevated%20eq%20true%20and%20expirationDateTime%20ne%20null%20or%20isElevated%20eq%20false
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="f52c7-173">C#</span><span class="sxs-lookup"><span data-stu-id="f52c7-173">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-privilegedroleassignments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f52c7-174">Javascript</span><span class="sxs-lookup"><span data-stu-id="f52c7-174">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-privilegedroleassignments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f52c7-175">目的-C</span><span class="sxs-lookup"><span data-stu-id="f52c7-175">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-privilegedroleassignments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="f52c7-176">Java</span><span class="sxs-lookup"><span data-stu-id="f52c7-176">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-privilegedroleassignments-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="f52c7-177">応答</span><span class="sxs-lookup"><span data-stu-id="f52c7-177">Response</span></span> 
<span data-ttu-id="f52c7-178">次の例は応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="f52c7-178">The following example shows the response.</span></span> <span data-ttu-id="f52c7-179">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="f52c7-179">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="f52c7-180">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="f52c7-180">All of the properties will be returned from an actual call.</span></span>
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
  ]
}
-->
