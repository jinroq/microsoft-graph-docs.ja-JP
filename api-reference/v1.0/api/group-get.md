---
title: グループを取得する
description: グループ オブジェクトのプロパティとリレーションシップを取得します。
ms.openlocfilehash: fbae878043580a9c5495b0462290e1da7af3bdd5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27022168"
---
# <a name="get-group"></a><span data-ttu-id="52558-103">グループを取得する</span><span class="sxs-lookup"><span data-stu-id="52558-103">Get group</span></span>
<span data-ttu-id="52558-104">グループ オブジェクトのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="52558-104">Get the properties and relationships of a group object.</span></span>

##### <a name="default-properties"></a><span data-ttu-id="52558-105">既定のプロパティ</span><span class="sxs-lookup"><span data-stu-id="52558-105">Default properties</span></span>

<span data-ttu-id="52558-p101">以下は、グループを取得または一覧表示するときに返されるプロパティの既定のセットを表します。これらは、利用可能なすべてのプロパティのサブセットです。</span><span class="sxs-lookup"><span data-stu-id="52558-p101">The following represent the default set of properties that are returned when getting or listing groups. These are a subset of all available properties.</span></span>

* <span data-ttu-id="52558-108">description</span><span class="sxs-lookup"><span data-stu-id="52558-108">description</span></span>
* <span data-ttu-id="52558-109">displayName</span><span class="sxs-lookup"><span data-stu-id="52558-109">displayName</span></span>
* <span data-ttu-id="52558-110">groupTypes</span><span class="sxs-lookup"><span data-stu-id="52558-110">groupTypes</span></span>
* <span data-ttu-id="52558-111">id</span><span class="sxs-lookup"><span data-stu-id="52558-111">id</span></span>
* <span data-ttu-id="52558-112">mail</span><span class="sxs-lookup"><span data-stu-id="52558-112">mail</span></span>
* <span data-ttu-id="52558-113">mailEnabled</span><span class="sxs-lookup"><span data-stu-id="52558-113">mailEnabled</span></span>
* <span data-ttu-id="52558-114">mailNickname</span><span class="sxs-lookup"><span data-stu-id="52558-114">mailNickname</span></span>
* <span data-ttu-id="52558-115">onPremisesLastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="52558-115">onPremisesLastSyncDateTime</span></span>
* <span data-ttu-id="52558-116">onPremisesSecurityIdentifier</span><span class="sxs-lookup"><span data-stu-id="52558-116">onPremisesSecurityIdentifier</span></span>
* <span data-ttu-id="52558-117">onPremisesSyncEnabled</span><span class="sxs-lookup"><span data-stu-id="52558-117">onPremisesSyncEnabled</span></span>
* <span data-ttu-id="52558-118">proxyAddresses</span><span class="sxs-lookup"><span data-stu-id="52558-118">proxyAddresses</span></span>
* <span data-ttu-id="52558-119">securityEnabled</span><span class="sxs-lookup"><span data-stu-id="52558-119">securityEnabled</span></span>
* <span data-ttu-id="52558-120">visibility</span><span class="sxs-lookup"><span data-stu-id="52558-120">visibility</span></span>

<span data-ttu-id="52558-121">次のグループ プロパティは既定では返されません。</span><span class="sxs-lookup"><span data-stu-id="52558-121">The following group properties are not returned by default:</span></span>

* <span data-ttu-id="52558-122">allowExternalSenders</span><span class="sxs-lookup"><span data-stu-id="52558-122">allowExternalSenders</span></span>
* <span data-ttu-id="52558-123">autoSubscribeNewMembers</span><span class="sxs-lookup"><span data-stu-id="52558-123">autoSubscribeNewMembers</span></span>
* <span data-ttu-id="52558-124">isSubscribedByMail</span><span class="sxs-lookup"><span data-stu-id="52558-124">isSubscribedByMail</span></span>
* <span data-ttu-id="52558-125">unseenCount</span><span class="sxs-lookup"><span data-stu-id="52558-125">unseenCount</span></span>

<span data-ttu-id="52558-p102">これらのプロパティを取得するには、**$select** クエリ パラメーターを使用します。次に、例を示します。</span><span class="sxs-lookup"><span data-stu-id="52558-p102">To get these properties, use the **$select** query parameter. The following are examples:</span></span> 

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/groups/c28c1cc9-e1ab-4c4d-98d1-d8fdf128b60f?$select=allowExternalSenders,autoSubscribeNewMembers,isSubscribedByMail,unseenCount

GET https://graph.microsoft.com/v1.0/groups/c28c1cc9-e1ab-4c4d-98d1-d8fdf128b60f?$select=description,allowExternalSenders
```


## <a name="permissions"></a><span data-ttu-id="52558-128">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="52558-128">Permissions</span></span>
<span data-ttu-id="52558-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="52558-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="52558-131">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="52558-131">Permission type</span></span>      | <span data-ttu-id="52558-132">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="52558-132">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="52558-133">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="52558-133">Delegated (work or school account)</span></span> | <span data-ttu-id="52558-134">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="52558-134">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="52558-135">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="52558-135">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="52558-136">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="52558-136">Not supported.</span></span>    |
|<span data-ttu-id="52558-137">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="52558-137">Application</span></span> | <span data-ttu-id="52558-138">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="52558-138">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="52558-139">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="52558-139">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="52558-140">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="52558-140">Optional query parameters</span></span>
<span data-ttu-id="52558-141">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="52558-141">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="52558-142">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="52558-142">Request headers</span></span>
| <span data-ttu-id="52558-143">名前</span><span class="sxs-lookup"><span data-stu-id="52558-143">Name</span></span>       | <span data-ttu-id="52558-144">型</span><span class="sxs-lookup"><span data-stu-id="52558-144">Type</span></span> | <span data-ttu-id="52558-145">説明</span><span class="sxs-lookup"><span data-stu-id="52558-145">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="52558-146">Authorization</span><span class="sxs-lookup"><span data-stu-id="52558-146">Authorization</span></span>  | <span data-ttu-id="52558-147">string</span><span class="sxs-lookup"><span data-stu-id="52558-147">string</span></span>  | <span data-ttu-id="52558-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="52558-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="52558-150">要求本文</span><span class="sxs-lookup"><span data-stu-id="52558-150">Request body</span></span>
<span data-ttu-id="52558-151">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="52558-151">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="52558-152">応答</span><span class="sxs-lookup"><span data-stu-id="52558-152">Response</span></span>
<span data-ttu-id="52558-153">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で[グループ](../resources/group.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="52558-153">If successful, this method returns a `200 OK` response code and [group](../resources/group.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="52558-154">例</span><span class="sxs-lookup"><span data-stu-id="52558-154">Example</span></span>
#### <a name="request"></a><span data-ttu-id="52558-155">要求</span><span class="sxs-lookup"><span data-stu-id="52558-155">Request</span></span>
<span data-ttu-id="52558-156">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="52558-156">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_group"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}
```

#### <a name="response"></a><span data-ttu-id="52558-157">応答</span><span class="sxs-lookup"><span data-stu-id="52558-157">Response</span></span>
<span data-ttu-id="52558-158">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="52558-158">The following is an example of the response.</span></span>

><span data-ttu-id="52558-159">**注:** ここに示す応答オブジェクトは、読みやすさの短縮される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="52558-159">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="52558-160">実際の呼び出しでは、前に示したように既定のプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="52558-160">The default properties will be returned from an actual call, as described before.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: xxx

{
  "id": "id-value",
  "description": "description-value",
  "displayName": "displayName-value",
  "groupTypes": [
    "groupTypes-value"
  ],
  "mail": "mail-value",
  "mailEnabled": true,
  "mailNickname": "mailNickname-value",
  "onPremisesLastSyncDateTime": "onPremisesLastSyncDateTime-value",
  "onPremisesSecurityIdentifier": "onPremisesSecurityIdentifier-value",
  "onPremisesSyncEnabled": true,
  "proxyAddresses": [
    "proxyAddresses-value"
   ],
   "securityEnabled": true,
   "visibility": "visibility-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get group",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
