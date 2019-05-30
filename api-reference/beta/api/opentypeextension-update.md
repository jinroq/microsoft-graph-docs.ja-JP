---
title: オープン拡張機能を更新する
description: 要求本文内のプロパティでオープン拡張機能 (openTypeExtension オブジェクト) を更新します。
localization_priority: Normal
author: dkershaw10
ms.openlocfilehash: 881a408d45418e4d267cea230121a90c4c4f3578
ms.sourcegitcommit: c0df90d66cb2072848d4bb0bf730c47a601b99ce
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/29/2019
ms.locfileid: "34536436"
---
# <a name="update-open-extension"></a><span data-ttu-id="deadc-103">オープン拡張機能を更新する</span><span class="sxs-lookup"><span data-stu-id="deadc-103">Update open extension</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="deadc-104">要求本文内のプロパティでオープン拡張機能 ([openTypeExtension](../resources/opentypeextension.md) オブジェクト) を更新します。</span><span class="sxs-lookup"><span data-stu-id="deadc-104">Update an open extension ([openTypeExtension](../resources/opentypeextension.md) object) with the properties in the request body:</span></span>

- <span data-ttu-id="deadc-105">要求本文内のプロパティが拡張情報内の既存のプロパティの名前と一致すると、拡張情報内のデータが更新されます。</span><span class="sxs-lookup"><span data-stu-id="deadc-105">If a property in the request body matches the name of an existing property in the extension, the data in the extension is updated.</span></span>
- <span data-ttu-id="deadc-106">一致しないと、このプロパティとそのデータは拡張情報に追加されます。</span><span class="sxs-lookup"><span data-stu-id="deadc-106">Otherwise that property and its data are added to the extension.</span></span> 

<span data-ttu-id="deadc-107">拡張機能内のデータは、プリミティブ型、またはプリミティブ型の配列にすることができます。</span><span class="sxs-lookup"><span data-stu-id="deadc-107">The data in an extension can be primitive types, or arrays of primitive types.</span></span>

## <a name="permissions"></a><span data-ttu-id="deadc-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="deadc-108">Permissions</span></span>

<span data-ttu-id="deadc-109">拡張機能が作成されたリソースと、要求されたアクセス許可の種類 (委任またはアプリケーション) に応じて、次の表で指定されているアクセス許可は、この API を呼び出すために必要な最低限の特権です。</span><span class="sxs-lookup"><span data-stu-id="deadc-109">Depending on the resource that the extension was created in and the permission type (delegated or application) requested, the permission specified in the following table is the least privileged required to call this API.</span></span> <span data-ttu-id="deadc-110">アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="deadc-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="deadc-111">サポートされているリソース</span><span class="sxs-lookup"><span data-stu-id="deadc-111">Supported resource</span></span> | <span data-ttu-id="deadc-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="deadc-112">Delegated (work or school account)</span></span> | <span data-ttu-id="deadc-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="deadc-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="deadc-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="deadc-114">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="deadc-115">device</span><span class="sxs-lookup"><span data-stu-id="deadc-115">device</span></span>](../resources/device.md) | <span data-ttu-id="deadc-116">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="deadc-116">Directory.AccessAsUser.All</span></span> | <span data-ttu-id="deadc-117">サポートされていません</span><span class="sxs-lookup"><span data-stu-id="deadc-117">Not supported</span></span> | <span data-ttu-id="deadc-118">Device.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="deadc-118">Device.ReadWrite.All</span></span> |
| [<span data-ttu-id="deadc-119">イベント</span><span class="sxs-lookup"><span data-stu-id="deadc-119">event</span></span>](../resources/event.md) | <span data-ttu-id="deadc-120">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="deadc-120">Calendars.ReadWrite</span></span> | <span data-ttu-id="deadc-121">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="deadc-121">Calendars.ReadWrite</span></span> | <span data-ttu-id="deadc-122">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="deadc-122">Calendars.ReadWrite</span></span> |
| [<span data-ttu-id="deadc-123">グループ</span><span class="sxs-lookup"><span data-stu-id="deadc-123">group</span></span>](../resources/group.md) | <span data-ttu-id="deadc-124">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="deadc-124">Group.ReadWrite.All</span></span> | <span data-ttu-id="deadc-125">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="deadc-125">Not supported</span></span> | <span data-ttu-id="deadc-126">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="deadc-126">Group.ReadWrite.All</span></span> |
| [<span data-ttu-id="deadc-127">グループ イベント</span><span class="sxs-lookup"><span data-stu-id="deadc-127">group event</span></span>](../resources/event.md) | <span data-ttu-id="deadc-128">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="deadc-128">Group.ReadWrite.All</span></span> | <span data-ttu-id="deadc-129">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="deadc-129">Not supported</span></span> | <span data-ttu-id="deadc-130">非サポート</span><span class="sxs-lookup"><span data-stu-id="deadc-130">Not supported</span></span> |
| [<span data-ttu-id="deadc-131">グループの投稿</span><span class="sxs-lookup"><span data-stu-id="deadc-131">group post</span></span>](../resources/post.md) | <span data-ttu-id="deadc-132">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="deadc-132">Group.ReadWrite.All</span></span> | <span data-ttu-id="deadc-133">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="deadc-133">Not supported</span></span> | <span data-ttu-id="deadc-134">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="deadc-134">Group.ReadWrite.All</span></span> |
| [<span data-ttu-id="deadc-135">メッセージ</span><span class="sxs-lookup"><span data-stu-id="deadc-135">message</span></span>](../resources/message.md) | <span data-ttu-id="deadc-136">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="deadc-136">Mail.ReadWrite</span></span> | <span data-ttu-id="deadc-137">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="deadc-137">Mail.ReadWrite</span></span> | <span data-ttu-id="deadc-138">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="deadc-138">Mail.ReadWrite</span></span> | 
| [<span data-ttu-id="deadc-139">組織</span><span class="sxs-lookup"><span data-stu-id="deadc-139">organization</span></span>](../resources/organization.md) | <span data-ttu-id="deadc-140">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="deadc-140">Directory.AccessAsUser.All</span></span> | <span data-ttu-id="deadc-141">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="deadc-141">Not supported</span></span> | <span data-ttu-id="deadc-142">非サポート</span><span class="sxs-lookup"><span data-stu-id="deadc-142">Not supported</span></span> |
| [<span data-ttu-id="deadc-143">個人用連絡先</span><span class="sxs-lookup"><span data-stu-id="deadc-143">personal contact</span></span>](../resources/contact.md) | <span data-ttu-id="deadc-144">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="deadc-144">Contacts.ReadWrite</span></span> | <span data-ttu-id="deadc-145">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="deadc-145">Contacts.ReadWrite</span></span> | <span data-ttu-id="deadc-146">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="deadc-146">Contacts.ReadWrite</span></span> |
| [<span data-ttu-id="deadc-147">user</span><span class="sxs-lookup"><span data-stu-id="deadc-147">user</span></span>](../resources/user.md) | <span data-ttu-id="deadc-148">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="deadc-148">User.ReadWrite.All</span></span> | <span data-ttu-id="deadc-149">User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="deadc-149">User.ReadWrite</span></span> | <span data-ttu-id="deadc-150">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="deadc-150">User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="deadc-151">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="deadc-151">HTTP request</span></span>

<span data-ttu-id="deadc-152">要求で、リソース インスタンスを識別し、そのインスタンスの **extensions** ナビゲーション プロパティを使用して拡張機能を識別し、その拡張インスタンスで `PATCH` を行います。</span><span class="sxs-lookup"><span data-stu-id="deadc-152">In the request, identify the resource instance, use the **extensions** navigation property of that instance to identify the extension, and do a `PATCH` on that extension instance.</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH /administrativeUnits/{Id}/extensions/{extensionId}
PATCH /devices/{Id}/extensions/{extensionId}
PATCH /users/{id|userPrincipalName}/events/{id}/extensions/{extensionId}
PATCH /groups/{id}/extensions/{extensionId}
PATCH /groups/{id}/events/{id}/extensions/{extensionId}
PATCH /groups/{id}/threads/{id}/posts/{id}/extensions/{extensionId}
PATCH /users/{id|userPrincipalName}/messages/{id}/extensions/{extensionId}
PATCH /organization/{Id}/extensions/{extensionId}
PATCH /users/{id|userPrincipalName}/contacts/{id}/extensions/{extensionId}
PATCH /users/{id|userPrincipalName}/extensions/{extensionId}
```

><span data-ttu-id="deadc-p102">**注:** 上記の構文は、含まれる拡張機能を更新するリソース インスタンスを特定する一般的な方法を示しています。こうしたリソース インスタンスを特定するために使用できる他の構文すべても、同様の方法でオープン拡張機能を更新できます。</span><span class="sxs-lookup"><span data-stu-id="deadc-p102">**Note:** The above syntax shows some common ways to identify a resource instance, in order to update an extension in it. All other syntax that allows you to identify these resource instances supports updating open extensions in them in a similar way.</span></span>

<span data-ttu-id="deadc-155">要求本文に、その拡張情報への変更や追加を行うための任意のカスタム データを含める方法については、[要求本文](#request-body)のセクションをご覧ください。</span><span class="sxs-lookup"><span data-stu-id="deadc-155">See the [Request body](#request-body) section about including in the request body any custom data to change or add to that extension.</span></span>

## <a name="path-parameters"></a><span data-ttu-id="deadc-156">パス パラメーター</span><span class="sxs-lookup"><span data-stu-id="deadc-156">Path parameters</span></span>
|<span data-ttu-id="deadc-157">**パラメーター**</span><span class="sxs-lookup"><span data-stu-id="deadc-157">**Parameter**</span></span>|<span data-ttu-id="deadc-158">**型**</span><span class="sxs-lookup"><span data-stu-id="deadc-158">**Type**</span></span>|<span data-ttu-id="deadc-159">**説明**</span><span class="sxs-lookup"><span data-stu-id="deadc-159">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="deadc-160">id</span><span class="sxs-lookup"><span data-stu-id="deadc-160">id</span></span>|<span data-ttu-id="deadc-161">string</span><span class="sxs-lookup"><span data-stu-id="deadc-161">string</span></span>|<span data-ttu-id="deadc-p103">対応するコレクションのインスタンスの一意識別子。必須。</span><span class="sxs-lookup"><span data-stu-id="deadc-p103">A unique identifier for an instance of the corresponding collection. Required.</span></span>|
|<span data-ttu-id="deadc-164">extensionId</span><span class="sxs-lookup"><span data-stu-id="deadc-164">extensionId</span></span>|<span data-ttu-id="deadc-165">string</span><span class="sxs-lookup"><span data-stu-id="deadc-165">string</span></span>|<span data-ttu-id="deadc-p104">これは、拡張情報の一意のテキスト識別子である拡張情報名、または拡張情報の種類と一意のテキスト識別子を連結した完全修飾名になります。完全修飾名は、拡張情報を作成したときに、`id` プロパティで返されます。必須。</span><span class="sxs-lookup"><span data-stu-id="deadc-p104">This can be an extension name which is a unique text identifier for an extension, or a fully qualified name which concatenates the extension type and unique text identifier. The fully qualified name is returned in the `id` property when you create the extension. Required.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="deadc-169">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="deadc-169">Request headers</span></span>
| <span data-ttu-id="deadc-170">名前</span><span class="sxs-lookup"><span data-stu-id="deadc-170">Name</span></span>       | <span data-ttu-id="deadc-171">値</span><span class="sxs-lookup"><span data-stu-id="deadc-171">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="deadc-172">Authorization</span><span class="sxs-lookup"><span data-stu-id="deadc-172">Authorization</span></span> | <span data-ttu-id="deadc-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="deadc-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="deadc-175">Content-Type</span><span class="sxs-lookup"><span data-stu-id="deadc-175">Content-Type</span></span> | <span data-ttu-id="deadc-176">application/json</span><span class="sxs-lookup"><span data-stu-id="deadc-176">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="deadc-177">要求本文</span><span class="sxs-lookup"><span data-stu-id="deadc-177">Request body</span></span>

<span data-ttu-id="deadc-p106">次に示す必須の名前/値のペアと、その拡張情報に変更を加えるデータまたは追加するデータとともに、[openTypeExtension](../resources/opentypeextension.md) オブジェクトの JSON 本文を指定します。JSON ペイロード内のデータは、プリミティブ型か、プリミティブ型の配列にすることができます。</span><span class="sxs-lookup"><span data-stu-id="deadc-p106">Provide a JSON body of an [openTypeExtension](../resources/opentypeextension.md) object, with the following required name-value pairs, and any custom data to change or add to that extension. The data in the JSON payload can be primitive types, or arrays of primitive types.</span></span>

| <span data-ttu-id="deadc-180">名前</span><span class="sxs-lookup"><span data-stu-id="deadc-180">Name</span></span>       | <span data-ttu-id="deadc-181">値</span><span class="sxs-lookup"><span data-stu-id="deadc-181">Value</span></span> |
|:---------------|:----------|
| <span data-ttu-id="deadc-182">@odata.type</span><span class="sxs-lookup"><span data-stu-id="deadc-182">@odata.type</span></span> | <span data-ttu-id="deadc-183">microsoft.graph.openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="deadc-183">microsoft.graph.openTypeExtension</span></span> |
| <span data-ttu-id="deadc-184">extensionName</span><span class="sxs-lookup"><span data-stu-id="deadc-184">extensionName</span></span> | <span data-ttu-id="deadc-185">%unique_string%</span><span class="sxs-lookup"><span data-stu-id="deadc-185">%unique_string%</span></span> |

## <a name="response"></a><span data-ttu-id="deadc-186">応答</span><span class="sxs-lookup"><span data-stu-id="deadc-186">Response</span></span>

<span data-ttu-id="deadc-187">成功した場合、このメソッドは `200 OK` 応答コードと、更新した [openTypeExtension](../resources/opentypeextension.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="deadc-187">If successful, this method returns a `200 OK` response code and the updated [openTypeExtension](../resources/opentypeextension.md) object.</span></span>


## <a name="example"></a><span data-ttu-id="deadc-188">例</span><span class="sxs-lookup"><span data-stu-id="deadc-188">Example</span></span>
#### <a name="request-1"></a><span data-ttu-id="deadc-189">要求 1</span><span class="sxs-lookup"><span data-stu-id="deadc-189">Request 1</span></span>

<span data-ttu-id="deadc-p107">最初の例では、メッセージ内の拡張情報を更新する方法を示します。この拡張情報は、最初に次の JSON ペイロードで表されます。</span><span class="sxs-lookup"><span data-stu-id="deadc-p107">The first example shows how to update an extension in a message. The extension is initially represented by the following JSON payload:</span></span>

<!-- { "blockType": "ignored" } -->
```http
{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Me/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions/$entity",
    "@odata.type": "#microsoft.graph.openTypeExtension",
    "@odata.id": "https://graph.microsoft.com/beta/users('ddfc984d-b826-40d7-b48b-57002df85e00@1717f226-49d1-4d0c-9d74-709fad6677b4')/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions
('Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral')",
    "extensionName": "Com.Contoso.Referral",
    "id": "Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral",
    "companyName": "Wingtip Toys",
    "dealValue": 500050,
    "expirationDate": "2015-12-03T10:00:00Z"
}
```

<span data-ttu-id="deadc-192">拡張情報は、その名前で参照できます。</span><span class="sxs-lookup"><span data-stu-id="deadc-192">You can reference the extension by its name:</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH https://graph.microsoft.com/beta/me/messages/AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===/extensions/Com.Contoso.Referral
```

<span data-ttu-id="deadc-193">また、拡張情報は、その完全修飾名でも参照できます。</span><span class="sxs-lookup"><span data-stu-id="deadc-193">Or you can reference the extension by its fully qualified name:</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH https://graph.microsoft.com/beta/me/messages/AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===/extensions/Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral
```

<span data-ttu-id="deadc-194">要求の例と以下の要求本文を使用して、上記の拡張情報を次のように更新できます。</span><span class="sxs-lookup"><span data-stu-id="deadc-194">You can use either example request and the following request body to update the above extension by:</span></span>
- <span data-ttu-id="deadc-195">`companyName` を `Wingtip Toys` から `Wingtip Toys (USA)` に変更する</span><span class="sxs-lookup"><span data-stu-id="deadc-195">Changing `companyName` from `Wingtip Toys` to `Wingtip Toys (USA)`</span></span>
- <span data-ttu-id="deadc-196">`dealValue` を `500050` から `500100` に変更する</span><span class="sxs-lookup"><span data-stu-id="deadc-196">Changing `dealValue` from `500050` to `500100`</span></span>
- <span data-ttu-id="deadc-197">新しいデータをカスタム プロパティ `updated` として追加する</span><span class="sxs-lookup"><span data-stu-id="deadc-197">Adding new data as the custom property `updated`</span></span>

<!-- { "blockType": "ignored" } -->
```http
{
    "@odata.type": "microsoft.graph.openTypeExtension",
    "extensionName": "Com.Contoso.Referral",
    "companyName": "Wingtip Toys (USA)",
    "dealValue": "500100",
    "expirationDate": "2015-12-03T10:00:00.000Z",
    "updated": "2015-10-29T11:00:00.000Z"
} 
```


#### <a name="response-1"></a><span data-ttu-id="deadc-198">応答 1</span><span class="sxs-lookup"><span data-stu-id="deadc-198">Response 1</span></span>

<span data-ttu-id="deadc-199">ここでは、拡張情報を参照するために使用する方法にかかわらず、同じになる応答を示します。</span><span class="sxs-lookup"><span data-stu-id="deadc-199">Here is the response which is the same regardless of the way used to reference the extension.</span></span>

<!-- { "blockType": "ignored" } -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Me/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions/$entity",
    "@odata.type": "#microsoft.graph.openTypeExtension",
    "@odata.id": "https://graph.microsoft.com/beta/users('ddfc984d-b826-40d7-b48b-57002df85e00@1717f226-49d1-4d0c-9d74-709fad6677b4')/messages('AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl===')/extensions
('Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral')",
    "id": "Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral",
    "extensionName": "Com.Contoso.Referral",
    "companyName": "Wingtip Toys (USA)",
    "dealValue": 500100,
    "expirationDate": "2015-12-03T10:00:00Z",
    "updated": "2015-10-29T11:00:00.000Z"
}
```

****

#### <a name="request-2"></a><span data-ttu-id="deadc-200">要求 2</span><span class="sxs-lookup"><span data-stu-id="deadc-200">Request 2</span></span>

<span data-ttu-id="deadc-p108">2 番目の例では、グループ投稿に含まれる拡張情報を更新する方法を示します。この拡張情報は、次の JSON ペイロード (`expirationDate` の値が `2015-07-03T13:04:00Z`) で最初に表されます。</span><span class="sxs-lookup"><span data-stu-id="deadc-p108">The second example shows how to update an extension in a group post. The extension is initially represented by the following JSON payload, with an `expirationDate` value of `2015-07-03T13:04:00Z`:</span></span>

<!-- { "blockType": "ignored" } -->
```http
{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#groups('37df2ff0-0de0-4c33-8aee-75289364aef6')/threads('AAQkADJizZJpEWwqDHsEpV_KA%3D%3D')/posts('AAMkADJiUg96QZUkA-ICwMubAADDEd7UAAA%3D')/extensions/$entity",
    "@odata.type": "#microsoft.graph.openTypeExtension",
    "id": "Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Estimate",
    "extensionName": "Com.Contoso.Estimate",
    "companyName": "Contoso",
    "expirationDate": "2015-07-03T13:04:00Z",
    "DealValue": 1010100,
    "Strings@odata.type": "#Collection(String)",
    "topPicks": [
        "Employees only",
        "Add spouse or guest",
        "Add family"
    ]
}
```

<span data-ttu-id="deadc-203">次に、`expirationDate` を `2016-07-30T11:00:00Z` に変更する要求と要求本文を示します。</span><span class="sxs-lookup"><span data-stu-id="deadc-203">The following is the request and request body to change the `expirationDate` to `2016-07-30T11:00:00Z`:</span></span>

<!-- {
  "blockType": "request",
  "name": "update_opentypeextension"
}-->
```http
PATCH https://graph.microsoft.com/beta/groups/37df2ff0-0de0-4c33-8aee-75289364aef6/threads/AAQkADJizZJpEWwqDHsEpV_KA==/posts/AAMkADJiUg96QZUkA-ICwMubAADDEd7UAAA=/extensions/Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Estimate
Content-type: application/json

{
   "@odata.type": "#microsoft.outlookServices.openTypeExtension",
   "extensionName": "Com.Contoso.Estimate",
   "companyName": "Contoso",
   "expirationDate": "2016-07-30T11:00:00.000Z",
   "DealValue": 1010100,
   "topPicks": [
       "Employees only",
       "Add spouse or guest",
       "Add family"
    ]
}
```

#### <a name="response-2"></a><span data-ttu-id="deadc-204">応答 2</span><span class="sxs-lookup"><span data-stu-id="deadc-204">Response 2</span></span>

<span data-ttu-id="deadc-205">ここでは、拡張情報内の更新された `expirationDate` を表示する 2 番目の例の応答を示します。</span><span class="sxs-lookup"><span data-stu-id="deadc-205">Here is the response of the second example which shows the updated `expirationDate` in the extension.</span></span>

<!-- {  
  "blockType": "response",  
  "truncated": true,  
  "@odata.type": "microsoft.graph.openTypeExtension"  
} --> 
```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#groups('37df2ff0-0de0-4c33-8aee-75289364aef6')/threads('AAQkADJizZJpEWwqDHsEpV_KA%3D%3D')/posts('AAMkADJiUg96QZUkA-ICwMubAADDEd7UAAA%3D')/extensions/$entity",
    "@odata.type": "#microsoft.graph.openTypeExtension",
    "id": "Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Estimate",
    "extensionName": "Com.Contoso.Estimate",
    "companyName": "Contoso",
    "expirationDate": "2016-07-30T11:00:00Z",
    "DealValue": 1010100,
    "Strings@odata.type": "#Collection(String)",
    "topPicks": [
        "Employees only",
        "Add spouse or guest",
        "Add family"
    ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="deadc-206">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="deadc-206">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="deadc-207">C#</span><span class="sxs-lookup"><span data-stu-id="deadc-207">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_opentypeextension-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="deadc-208">Javascript</span><span class="sxs-lookup"><span data-stu-id="deadc-208">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_opentypeextension-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- This page was manually created. -->
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update opentypeextension",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/opentypeextension-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/opentypeextension-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
