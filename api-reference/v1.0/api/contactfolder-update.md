---
title: Update contactfolder
description: contactfolder オブジェクトのプロパティを更新します。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 39a0869757fe42fd4502b194b84c3fe3e3edad68
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32566109"
---
# <a name="update-contactfolder"></a><span data-ttu-id="640be-103">Update contactfolder</span><span class="sxs-lookup"><span data-stu-id="640be-103">Update contactfolder</span></span>

<span data-ttu-id="640be-104">contactfolder オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="640be-104">Update the properties of contactfolder object.</span></span>
## <a name="permissions"></a><span data-ttu-id="640be-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="640be-105">Permissions</span></span>
<span data-ttu-id="640be-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="640be-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="640be-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="640be-108">Permission type</span></span>      | <span data-ttu-id="640be-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="640be-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="640be-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="640be-110">Delegated (work or school account)</span></span> | <span data-ttu-id="640be-111">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="640be-111">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="640be-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="640be-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="640be-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="640be-113">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="640be-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="640be-114">Application</span></span> | <span data-ttu-id="640be-115">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="640be-115">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="640be-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="640be-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/contactFolders/{id}
PATCH /users/{id | userPrincipalName}/contactFolders/{id}
```
## <a name="request-headers"></a><span data-ttu-id="640be-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="640be-117">Request headers</span></span>
| <span data-ttu-id="640be-118">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="640be-118">Header</span></span>       | <span data-ttu-id="640be-119">値</span><span class="sxs-lookup"><span data-stu-id="640be-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="640be-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="640be-120">Authorization</span></span>  | <span data-ttu-id="640be-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="640be-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="640be-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="640be-123">Content-Type</span></span>  | <span data-ttu-id="640be-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="640be-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="640be-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="640be-126">Request body</span></span>
<span data-ttu-id="640be-p104">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="640be-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="640be-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="640be-130">Property</span></span>     | <span data-ttu-id="640be-131">型</span><span class="sxs-lookup"><span data-stu-id="640be-131">Type</span></span>   |<span data-ttu-id="640be-132">説明</span><span class="sxs-lookup"><span data-stu-id="640be-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="640be-133">displayName</span><span class="sxs-lookup"><span data-stu-id="640be-133">displayName</span></span>|<span data-ttu-id="640be-134">String</span><span class="sxs-lookup"><span data-stu-id="640be-134">String</span></span>|<span data-ttu-id="640be-135">フォルダーの表示名。</span><span class="sxs-lookup"><span data-stu-id="640be-135">The folder's display name.</span></span>|
|<span data-ttu-id="640be-136">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="640be-136">parentFolderId</span></span>|<span data-ttu-id="640be-137">String</span><span class="sxs-lookup"><span data-stu-id="640be-137">String</span></span>|<span data-ttu-id="640be-138">フォルダーの親フォルダーの ID。</span><span class="sxs-lookup"><span data-stu-id="640be-138">The ID of the folder's parent folder.</span></span>|

## <a name="response"></a><span data-ttu-id="640be-139">応答</span><span class="sxs-lookup"><span data-stu-id="640be-139">Response</span></span>

<span data-ttu-id="640be-140">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で、更新された [contactFolder](../resources/contactfolder.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="640be-140">If successful, this method returns a `200 OK` response code and updated [contactFolder](../resources/contactfolder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="640be-141">例</span><span class="sxs-lookup"><span data-stu-id="640be-141">Example</span></span>
##### <a name="request"></a><span data-ttu-id="640be-142">要求</span><span class="sxs-lookup"><span data-stu-id="640be-142">Request</span></span>
<span data-ttu-id="640be-143">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="640be-143">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_contactfolder"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/contactFolders/{id}
Content-type: application/json
Content-length: 84

{
  "parentFolderId": "parentFolderId-value",
  "displayName": "displayName-value"
}
```
##### <a name="response"></a><span data-ttu-id="640be-144">応答</span><span class="sxs-lookup"><span data-stu-id="640be-144">Response</span></span>
<span data-ttu-id="640be-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="640be-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contactFolder"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 104

{
  "parentFolderId": "parentFolderId-value",
  "displayName": "displayName-value",
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update contactfolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
