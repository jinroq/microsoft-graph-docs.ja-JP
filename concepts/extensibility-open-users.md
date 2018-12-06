---
title: オープン拡張機能を使用してカスタム データをユーザーに追加する
description: '*オープン拡張機能*の使用方法について、具体例を使ってデモンストレーションします。 '
ms.openlocfilehash: b2ff767e9eb0762ec3600166328d2bb0c5218936
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27092539"
---
# <a name="add-custom-data-to-users-using-open-extensions"></a><span data-ttu-id="1c6c1-103">オープン拡張機能を使用してカスタム データをユーザーに追加する</span><span class="sxs-lookup"><span data-stu-id="1c6c1-103">Add custom data to users using open extensions</span></span>
<span data-ttu-id="1c6c1-104">*オープン拡張機能*の使用方法について、具体例を使ってデモンストレーションします。</span><span class="sxs-lookup"><span data-stu-id="1c6c1-104">We're going to walk you through an example to demonstrate how to use *open extensions*.</span></span> 

<span data-ttu-id="1c6c1-p101">デスクトップやモバイルなど、多種のクライアント プラットフォームで利用できるアプリケーションをビルドしているとします。アプリにサインインするときのデバイスに関係なく一貫性を確保できるように、ユーザー自身で UI エクスペリエンスを構成できるようにしたいと考えています。これは、ほとんどのアプリで一般的な要件です。</span><span class="sxs-lookup"><span data-stu-id="1c6c1-p101">Imagine you're building an application that is available on lots of different client platforms, such as desktop and mobile.  You want to let users configure their UI experience so it’s consistent no matter which device they use to sign in to your app. This is a common requirement for most apps.</span></span> 

<span data-ttu-id="1c6c1-108">このシナリオでは、以下の操作を行う方法を紹介します。</span><span class="sxs-lookup"><span data-stu-id="1c6c1-108">For this scenario, we're going to show you how to:</span></span>

1. <span data-ttu-id="1c6c1-109">ユーザーに関する何らかのローミング プロファイル情報を表すオープン拡張機能を追加します。</span><span class="sxs-lookup"><span data-stu-id="1c6c1-109">Add an open extension representing some roaming profile information about the user.</span></span>
2. <span data-ttu-id="1c6c1-110">ユーザーに対してクエリを実行し、ローミング プロファイルを返します。</span><span class="sxs-lookup"><span data-stu-id="1c6c1-110">Query the user and return the roaming profile.</span></span>
3. <span data-ttu-id="1c6c1-111">ユーザーのローミング プロファイル情報 (オープン拡張機能値) を変更します。</span><span class="sxs-lookup"><span data-stu-id="1c6c1-111">Change the user's roaming profile information (the open extension value).</span></span>
4. <span data-ttu-id="1c6c1-112">ユーザーのローミング プロファイル情報を削除します。</span><span class="sxs-lookup"><span data-stu-id="1c6c1-112">Delete the user's roaming profile information.</span></span>

><span data-ttu-id="1c6c1-p102">**注:** このトピックでは、*user* リソースにおいてオープン拡張機能を追加、読み取り、更新、削除する方法を示します。これらの方法は、*administrativeUnit*、*contact*、*device*、*event*、*group*、*group event*、*group post*、*organizaton* の各リソース型でもサポートされています。</span><span class="sxs-lookup"><span data-stu-id="1c6c1-p102">**Note:** This topic shows you how to add, read, update and delete open extensions on a *user* resource.  These methods are also supported for the *administrativeUnit*, *contact*, *device*, *event*, *group*, *group event*, *group post* and *organizaton* resource types.</span></span>  
<span data-ttu-id="1c6c1-p103">これらのリソース型のいずれかを使用して、次の例の要求を簡単に更新できます。次の例に示されている応答は、わかりやすくするために途中までしか示されていない場合があります。</span><span class="sxs-lookup"><span data-stu-id="1c6c1-p103">Simply update the example requests below using any of those resource types. The responses shown in the examples below may be truncated for brevity.</span></span> 

## <a name="1-add-roaming-profile-information"></a><span data-ttu-id="1c6c1-117">1.ローミング プロファイル情報を追加する</span><span class="sxs-lookup"><span data-stu-id="1c6c1-117">1. Add roaming profile information</span></span>
<span data-ttu-id="1c6c1-p104">ユーザーがアプリにサインインし、アプリの外観を構成します。これらのアプリ設定はローミングされ、アプリにサインインするためにユーザーが使用するデバイスに関わらず同じエクスペリエンスになるようにする必要があります。ここでは、ユーザーのリソースにローミング プロファイル情報を追加する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="1c6c1-p104">The user signs in to the app and configures the look and feel of the app.  These app settings should roam so that the user gets the same experience on whatever device they sign in to the app from.  Here we'll see how to add the roaming profile information to a user resource.</span></span>

##### <a name="request"></a><span data-ttu-id="1c6c1-121">要求</span><span class="sxs-lookup"><span data-stu-id="1c6c1-121">Request</span></span>
```http
POST https://graph.microsoft.com/v1.0/me/extensions
Content-type: application/json
{
    "@odata.type":"microsoft.graph.openTypeExtension",
    "extensionName":"com.contoso.roamingSettings",
    "theme":"dark",
    "color":"purple",
    "lang":"Japanese"
}
```
##### <a name="response"></a><span data-ttu-id="1c6c1-122">応答</span><span class="sxs-lookup"><span data-stu-id="1c6c1-122">Response</span></span>
```http
HTTP/1.1 201 Created
Content-Type: application/json
Content-length: 420

{
    "@odata.type": "#microsoft.graph.openTypeExtension",
    "extensionName": "com.contoso.roamingSettings",
    "id": "com.contoso.roamingSettings",
    "theme": "dark",
    "color": "purple",
    "lang": "Japanese"
}
```

## <a name="2-retrieve-roaming-profile-information"></a><span data-ttu-id="1c6c1-123">2.ローミング プロファイル情報を取得する</span><span class="sxs-lookup"><span data-stu-id="1c6c1-123">2. Retrieve roaming profile information</span></span>
<span data-ttu-id="1c6c1-p105">ユーザーが別のデバイスからアプリにサインインするときに、アプリはユーザーのプロファイル詳細とローミング設定を取得できます。これは、ユーザーのリソースを取得し、拡張ナビゲーション プロパティを展開することによって行えます。</span><span class="sxs-lookup"><span data-stu-id="1c6c1-p105">When the user signs in to the app from another device, the app can retrieve the user's profile details as well as their roaming settings. This can be done by getting the user's resource and expanding the extension navigation property.</span></span>

##### <a name="request"></a><span data-ttu-id="1c6c1-126">要求</span><span class="sxs-lookup"><span data-stu-id="1c6c1-126">Request</span></span>
```http
GET https://graph.microsoft.com/v1.0/me?$select=id,displayName,mail,mobilePhone&$expand=extensions
```
##### <a name="response"></a><span data-ttu-id="1c6c1-127">応答</span><span class="sxs-lookup"><span data-stu-id="1c6c1-127">Response</span></span>
```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-length: 420

{
    "id": "84b80893-8749-40a3-97b7-68513b600544",
    "displayName": "John Smith",
    "mail": "john@contoso.com",
    "mobilePhone": "1-555-6589",
    "extensions": [
        {
            "@odata.type": "#microsoft.graph.openTypeExtension",
            "extensionName": "com.contoso.roamingSettings",
            "id": "com.contoso.roamingSettings",
            "theme": "dark",
            "color": "purple",
            "lang": "Japanese"
        }
    ]
}
```
><span data-ttu-id="1c6c1-128">**注:** 複数の拡張機能がある場合、対象の拡張機能を取得するために *id* でフィルター処理できます。</span><span class="sxs-lookup"><span data-stu-id="1c6c1-128">**Note:** If you have multiple extensions, you can filter on the *id* to get the extension that you are interested in.</span></span>

## <a name="3-change-roaming-profile-information"></a><span data-ttu-id="1c6c1-129">3.ローミング プロファイル情報を変更する</span><span class="sxs-lookup"><span data-stu-id="1c6c1-129">3. Change roaming profile information</span></span>
<span data-ttu-id="1c6c1-p106">ユーザーは、ローミング プロファイル情報を変更することができます。オープン拡張機能の値で ```PATCH``` を使用して更新できます。</span><span class="sxs-lookup"><span data-stu-id="1c6c1-p106">The user may choose to change their roaming profile information.  This update can be done with a ```PATCH``` on the open extension value.</span></span> 

##### <a name="request"></a><span data-ttu-id="1c6c1-132">要求</span><span class="sxs-lookup"><span data-stu-id="1c6c1-132">Request</span></span>
```http
PATCH https://graph.microsoft.com/v1.0/me/extensions/com.contoso.roamingSettings
Content-type: application/json
{
    "theme":"light",
    "color":"yellow",
    "lang":"Swahili"
}
```

##### <a name="response"></a><span data-ttu-id="1c6c1-133">応答</span><span class="sxs-lookup"><span data-stu-id="1c6c1-133">Response</span></span>
```
HTTP/1.1 204 No content
```

## <a name="4-delete-a-users-roaming-profile"></a><span data-ttu-id="1c6c1-134">4.ユーザーのローミング プロファイルを削除する</span><span class="sxs-lookup"><span data-stu-id="1c6c1-134">4. Delete a user's roaming profile</span></span>
<span data-ttu-id="1c6c1-p107">ローミング プロファイルがもはや不要であるとユーザーが判断する場合、削除できます。オープン拡張機能の値で ```DELETE``` 要求を使用して行えます。</span><span class="sxs-lookup"><span data-stu-id="1c6c1-p107">The user decides that they don't want a roaming profile anymore, so they delete it. This can be done with a ```DELETE``` request on the open extension value.</span></span>

##### <a name="request"></a><span data-ttu-id="1c6c1-137">要求</span><span class="sxs-lookup"><span data-stu-id="1c6c1-137">Request</span></span>
```http
DELETE https://graph.microsoft.com/v1.0/me/extensions/com.contoso.roamingSettings
```

##### <a name="response"></a><span data-ttu-id="1c6c1-138">応答</span><span class="sxs-lookup"><span data-stu-id="1c6c1-138">Response</span></span>
```
HTTP/1.1 204 No content
```

## <a name="see-also"></a><span data-ttu-id="1c6c1-139">関連項目</span><span class="sxs-lookup"><span data-stu-id="1c6c1-139">See also</span></span>

- [<span data-ttu-id="1c6c1-140">拡張機能を使用してカスタム データをリソースに追加する</span><span class="sxs-lookup"><span data-stu-id="1c6c1-140">Add custom data to resources using extensions</span></span>](extensibility-overview.md)
- [<span data-ttu-id="1c6c1-141">スキーマ拡張機能を使用したグループへのカスタム データの追加</span><span class="sxs-lookup"><span data-stu-id="1c6c1-141">Add custom data to groups using schema extensions</span></span>](extensibility-schema-groups.md)
- [<span data-ttu-id="1c6c1-142">openTypeExtension リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="1c6c1-142">openTypeExtension resource type</span></span>](/graph/api/resources/opentypeextension?view=graph-rest-1.0)
- [<span data-ttu-id="1c6c1-143">オープン拡張機能を作成する</span><span class="sxs-lookup"><span data-stu-id="1c6c1-143">Create open extension</span></span>](/graph/api/opentypeextension-post-opentypeextension?view=graph-rest-1.0)
- [<span data-ttu-id="1c6c1-144">オープン拡張機能を取得する</span><span class="sxs-lookup"><span data-stu-id="1c6c1-144">Get open extension</span></span>](/graph/api/opentypeextension-get?view=graph-rest-1.0)
- [<span data-ttu-id="1c6c1-145">オープン拡張機能を更新する</span><span class="sxs-lookup"><span data-stu-id="1c6c1-145">Update open extension</span></span>](/graph/api/opentypeextension-update?view=graph-rest-1.0)
- [<span data-ttu-id="1c6c1-146">オープン拡張機能を削除する</span><span class="sxs-lookup"><span data-stu-id="1c6c1-146">Delete open extension</span></span>](/graph/api/opentypeextension-delete?view=graph-rest-1.0)