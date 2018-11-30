---
title: グループを取得する
description: グループ オブジェクトのプロパティとリレーションシップを取得します。
ms.openlocfilehash: 5bd4635e3eb9004a33c60fee0c802e77fa15a709
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073965"
---
# <a name="get-group"></a><span data-ttu-id="99993-103">グループを取得する</span><span class="sxs-lookup"><span data-stu-id="99993-103">Get group</span></span>

> <span data-ttu-id="99993-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="99993-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="99993-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="99993-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="99993-106">プロパティと[グループ](../resources/group.md)のオブジェクトの関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="99993-106">Get the properties and relationships of a [group](../resources/group.md) object.</span></span>

##### <a name="default-properties"></a><span data-ttu-id="99993-107">既定のプロパティ</span><span class="sxs-lookup"><span data-stu-id="99993-107">Default properties</span></span>

<span data-ttu-id="99993-p102">以下は、グループを取得または一覧表示するときに返されるプロパティの既定のセットを表します。これらは、利用可能なすべてのプロパティのサブセットです。</span><span class="sxs-lookup"><span data-stu-id="99993-p102">The following represent the default set of properties that are returned when getting or listing groups. These are a subset of all available properties.</span></span> 

* <span data-ttu-id="99993-110">分類</span><span class="sxs-lookup"><span data-stu-id="99993-110">classification</span></span>
* <span data-ttu-id="99993-111">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="99993-111">createdDateTime</span></span>
* <span data-ttu-id="99993-112">description</span><span class="sxs-lookup"><span data-stu-id="99993-112">description</span></span>
* <span data-ttu-id="99993-113">displayName</span><span class="sxs-lookup"><span data-stu-id="99993-113">displayName</span></span>
* <span data-ttu-id="99993-114">groupTypes</span><span class="sxs-lookup"><span data-stu-id="99993-114">groupTypes</span></span>
* <span data-ttu-id="99993-115">id</span><span class="sxs-lookup"><span data-stu-id="99993-115">id</span></span>
* <span data-ttu-id="99993-116">mail</span><span class="sxs-lookup"><span data-stu-id="99993-116">mail</span></span>
* <span data-ttu-id="99993-117">mailEnabled</span><span class="sxs-lookup"><span data-stu-id="99993-117">mailEnabled</span></span>
* <span data-ttu-id="99993-118">mailNickname</span><span class="sxs-lookup"><span data-stu-id="99993-118">mailNickname</span></span>
* <span data-ttu-id="99993-119">membershipRule</span><span class="sxs-lookup"><span data-stu-id="99993-119">membershipRule</span></span>
* <span data-ttu-id="99993-120">membershipRuleProcessingState</span><span class="sxs-lookup"><span data-stu-id="99993-120">membershipRuleProcessingState</span></span>
* <span data-ttu-id="99993-121">onPremisesLastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="99993-121">onPremisesLastSyncDateTime</span></span>
* <span data-ttu-id="99993-122">onPremisesSecurityIdentifier</span><span class="sxs-lookup"><span data-stu-id="99993-122">onPremisesSecurityIdentifier</span></span>
* <span data-ttu-id="99993-123">onPremisesSyncEnabled</span><span class="sxs-lookup"><span data-stu-id="99993-123">onPremisesSyncEnabled</span></span>
* <span data-ttu-id="99993-124">preferredLanguage - サポートされていません。このプロパティの値が設定とすることはできません`null`が呼び出されるとします。</span><span class="sxs-lookup"><span data-stu-id="99993-124">preferredLanguage - Not supported; a value for this property cannot be set and returns `null` when called.</span></span>
* <span data-ttu-id="99993-125">proxyAddresses</span><span class="sxs-lookup"><span data-stu-id="99993-125">proxyAddresses</span></span>
* <span data-ttu-id="99993-126">renewedDateTime</span><span class="sxs-lookup"><span data-stu-id="99993-126">renewedDateTime</span></span>
* <span data-ttu-id="99993-127">securityEnabled</span><span class="sxs-lookup"><span data-stu-id="99993-127">securityEnabled</span></span>
* <span data-ttu-id="99993-128">theme</span><span class="sxs-lookup"><span data-stu-id="99993-128">theme</span></span>
* <span data-ttu-id="99993-129">visibility</span><span class="sxs-lookup"><span data-stu-id="99993-129">visibility</span></span>

<span data-ttu-id="99993-130">次のグループ プロパティは既定では返されません。</span><span class="sxs-lookup"><span data-stu-id="99993-130">The following group properties are not returned by default:</span></span>

* <span data-ttu-id="99993-131">accessType</span><span class="sxs-lookup"><span data-stu-id="99993-131">accessType</span></span>
* <span data-ttu-id="99993-132">allowExternalSenders</span><span class="sxs-lookup"><span data-stu-id="99993-132">allowExternalSenders</span></span>
* <span data-ttu-id="99993-133">autoSubscribeNewMembers</span><span class="sxs-lookup"><span data-stu-id="99993-133">autoSubscribeNewMembers</span></span>
* <span data-ttu-id="99993-134">hasMembersWithLicenseErrors</span><span class="sxs-lookup"><span data-stu-id="99993-134">hasMembersWithLicenseErrors</span></span>
* <span data-ttu-id="99993-135">isSubscribedByMail</span><span class="sxs-lookup"><span data-stu-id="99993-135">isSubscribedByMail</span></span>
* <span data-ttu-id="99993-136">isFavorite</span><span class="sxs-lookup"><span data-stu-id="99993-136">isFavorite</span></span>
* <span data-ttu-id="99993-137">unseenConversationsCount</span><span class="sxs-lookup"><span data-stu-id="99993-137">unseenConversationsCount</span></span>
* <span data-ttu-id="99993-138">unseenCount</span><span class="sxs-lookup"><span data-stu-id="99993-138">unseenCount</span></span>
* <span data-ttu-id="99993-139">unseenMessagesCount</span><span class="sxs-lookup"><span data-stu-id="99993-139">unseenMessagesCount</span></span>

<span data-ttu-id="99993-140">( **IsFavorite**および**hasMembersWithLicenseErrors**) を除くこれらのプロパティを取得するを使用して、`$select`パラメーターのクエリを実行します。</span><span class="sxs-lookup"><span data-stu-id="99993-140">To get these properties (except **isFavorite** and **hasMembersWithLicenseErrors**), use the `$select` query parameter.</span></span> <span data-ttu-id="99993-141">次に、例を示します。</span><span class="sxs-lookup"><span data-stu-id="99993-141">The following are examples:</span></span> 

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/groups/c28c1cc9-e1ab-4c4d-98d1-d8fdf128b60f?$select=allowExternalSenders,autoSubscribeNewMembers,isSubscribedByMail,unseenCount

GET https://graph.microsoft.com/beta/groups/c28c1cc9-e1ab-4c4d-98d1-d8fdf128b60f?$select=description,allowExternalSenders
```

<span data-ttu-id="99993-142">ライセンス エラーのあるメンバーを含むグループを返すには、 **$filter**クエリ パラメーターを使用します。</span><span class="sxs-lookup"><span data-stu-id="99993-142">To return groups containing members with license errors, use the **$filter** query parameter:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET GET https://graph.microsoft.com/beta/groups?$filter=hasMembersWithLicenseErrors+eq+true
```

<span data-ttu-id="99993-143">**グループ**・ リソースは、[拡張機能](/graph/extensibility-overview)をサポートするため使用することも、 `GET` 、**グループ**のインスタンスのカスタム プロパティと拡張機能のデータを取得する操作です。</span><span class="sxs-lookup"><span data-stu-id="99993-143">Since the **group** resource supports [extensions](/graph/extensibility-overview), you can also use the `GET` operation to get custom properties and extension data in a **group** instance.</span></span>

## <a name="permissions"></a><span data-ttu-id="99993-144">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="99993-144">Permissions</span></span>
<span data-ttu-id="99993-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="99993-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="99993-147">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="99993-147">Permission type</span></span>      | <span data-ttu-id="99993-148">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="99993-148">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="99993-149">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="99993-149">Delegated (work or school account)</span></span> | <span data-ttu-id="99993-150">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="99993-150">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="99993-151">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="99993-151">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="99993-152">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="99993-152">Not supported.</span></span>    |
|<span data-ttu-id="99993-153">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="99993-153">Application</span></span> | <span data-ttu-id="99993-154">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="99993-154">Group.Read.All, Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="99993-155">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="99993-155">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="99993-156">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="99993-156">Optional query parameters</span></span>
<span data-ttu-id="99993-157">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="99993-157">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="99993-158">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="99993-158">Request headers</span></span>
| <span data-ttu-id="99993-159">名前</span><span class="sxs-lookup"><span data-stu-id="99993-159">Name</span></span>       | <span data-ttu-id="99993-160">型</span><span class="sxs-lookup"><span data-stu-id="99993-160">Type</span></span> | <span data-ttu-id="99993-161">説明</span><span class="sxs-lookup"><span data-stu-id="99993-161">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="99993-162">Authorization</span><span class="sxs-lookup"><span data-stu-id="99993-162">Authorization</span></span>  | <span data-ttu-id="99993-163">string</span><span class="sxs-lookup"><span data-stu-id="99993-163">string</span></span>  | <span data-ttu-id="99993-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="99993-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="99993-166">要求本文</span><span class="sxs-lookup"><span data-stu-id="99993-166">Request body</span></span>
<span data-ttu-id="99993-167">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="99993-167">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="99993-168">応答</span><span class="sxs-lookup"><span data-stu-id="99993-168">Response</span></span>
<span data-ttu-id="99993-169">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で[グループ](../resources/group.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="99993-169">If successful, this method returns a `200 OK` response code and [group](../resources/group.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="99993-170">例</span><span class="sxs-lookup"><span data-stu-id="99993-170">Example</span></span>
### <a name="request"></a><span data-ttu-id="99993-171">要求</span><span class="sxs-lookup"><span data-stu-id="99993-171">Request</span></span>
<span data-ttu-id="99993-172">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="99993-172">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_group"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}
```

### <a name="response"></a><span data-ttu-id="99993-173">応答</span><span class="sxs-lookup"><span data-stu-id="99993-173">Response</span></span>
<span data-ttu-id="99993-174">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="99993-174">The following is an example of the response.</span></span> 
><span data-ttu-id="99993-175">**注:** ここに示す応答オブジェクトは、読みやすさの短縮される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="99993-175">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="99993-176">実際の呼び出しでは、前に示したように既定のプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="99993-176">The default properties will be returned from an actual call, as described before.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="99993-177">関連項目</span><span class="sxs-lookup"><span data-stu-id="99993-177">See also</span></span>

- [<span data-ttu-id="99993-178">拡張機能を使用してカスタム データをリソースに追加する</span><span class="sxs-lookup"><span data-stu-id="99993-178">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="99993-179">オープン拡張機能を使用してカスタム データをユーザーに追加する</span><span class="sxs-lookup"><span data-stu-id="99993-179">Add custom data to users using open extensions</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="99993-180">スキーマ拡張機能を使用したグループへのカスタム データの追加</span><span class="sxs-lookup"><span data-stu-id="99993-180">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get group",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
