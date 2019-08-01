---
title: multiValueLegacyExtendedProperty を取得する
description: '[] を展開します。'
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: c8ca94f253b2949dc25c6cacf8ccdef516827a9d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36022804"
---
# <a name="get-multivaluelegacyextendedproperty"></a><span data-ttu-id="07c18-103">multiValueLegacyExtendedProperty を取得する</span><span class="sxs-lookup"><span data-stu-id="07c18-103">Get multiValueLegacyExtendedProperty</span></span>

<span data-ttu-id="07c18-104">`$expand` を使用して、複数値の拡張プロパティを含むリソース インスタンスを取得します。</span><span class="sxs-lookup"><span data-stu-id="07c18-104">Get a resource instance that contains a multi-value extended property by using `$expand`.</span></span>

<span data-ttu-id="07c18-105">クエリ パラメーター `$expand` を使用すると、指示された拡張プロパティで展開された特定のインスタンスを取得できます。</span><span class="sxs-lookup"><span data-stu-id="07c18-105">Using the query parameter `$expand` allows you to get the specified instance expanded with the indicated extended property.</span></span> <span data-ttu-id="07c18-106">これは、現時点で、拡張プロパティを表す [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) オブジェクトを取得する唯一の方法です。</span><span class="sxs-lookup"><span data-stu-id="07c18-106">This is currently the only way to get the [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) object that represents an extended property.</span></span>

<span data-ttu-id="07c18-107">次のユーザー リソースがサポートされます。</span><span class="sxs-lookup"><span data-stu-id="07c18-107">The following user resources are supported:</span></span>

- [<span data-ttu-id="07c18-108">calendar</span><span class="sxs-lookup"><span data-stu-id="07c18-108">calendar</span></span>](../resources/calendar.md)
- [<span data-ttu-id="07c18-109">contact</span><span class="sxs-lookup"><span data-stu-id="07c18-109">contact</span></span>](../resources/contact.md)
- [<span data-ttu-id="07c18-110">contactFolder</span><span class="sxs-lookup"><span data-stu-id="07c18-110">contactFolder</span></span>](../resources/contactfolder.md) 
- [<span data-ttu-id="07c18-111">event</span><span class="sxs-lookup"><span data-stu-id="07c18-111">event</span></span>](../resources/event.md)
- [<span data-ttu-id="07c18-112">mailFolder</span><span class="sxs-lookup"><span data-stu-id="07c18-112">mailFolder</span></span>](../resources/mailfolder.md)
- [<span data-ttu-id="07c18-113">message</span><span class="sxs-lookup"><span data-stu-id="07c18-113">message</span></span>](../resources/message.md) 

<span data-ttu-id="07c18-114">次のグループ リソースもサポートされます。</span><span class="sxs-lookup"><span data-stu-id="07c18-114">As well as the following group resources:</span></span>

- <span data-ttu-id="07c18-115">グループ [calendar](../resources/calendar.md)</span><span class="sxs-lookup"><span data-stu-id="07c18-115">group [calendar](../resources/calendar.md)</span></span>
- <span data-ttu-id="07c18-116">グループ [event](../resources/event.md)</span><span class="sxs-lookup"><span data-stu-id="07c18-116">group [event](../resources/event.md)</span></span>
- <span data-ttu-id="07c18-117">グループ [post](../resources/post.md)</span><span class="sxs-lookup"><span data-stu-id="07c18-117">group [post](../resources/post.md)</span></span>

<span data-ttu-id="07c18-118">オープン拡張機能または拡張プロパティを使用するのに適した状況と、拡張プロパティを指定する方法の詳細については、「[拡張プロパティの概要](../resources/extended-properties-overview.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="07c18-118">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="07c18-119">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="07c18-119">Permissions</span></span>
<span data-ttu-id="07c18-120">この API を呼び出すには、拡張プロパティの取得元のリソースと、要求したアクセス許可の種類 (委任またはアプリケーション) に応じて、次の表で指定されているアクセス許可が最低限必要です。</span><span class="sxs-lookup"><span data-stu-id="07c18-120">Depending on the resource you're getting the extended property from and the permission type (delegated or application) you request, the permission specified in the following table is the minimum required to call this API.</span></span> <span data-ttu-id="07c18-121">アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="07c18-121">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="07c18-122">サポートされているリソース</span><span class="sxs-lookup"><span data-stu-id="07c18-122">Supported resource</span></span> | <span data-ttu-id="07c18-123">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="07c18-123">Delegated (work or school account)</span></span> | <span data-ttu-id="07c18-124">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="07c18-124">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="07c18-125">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="07c18-125">Application</span></span> |
|:-----|:-----|:-----|:-----|
| [<span data-ttu-id="07c18-126">calendar</span><span class="sxs-lookup"><span data-stu-id="07c18-126">calendar</span></span>](../resources/calendar.md) | <span data-ttu-id="07c18-127">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="07c18-127">Calendars.Read</span></span> | <span data-ttu-id="07c18-128">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="07c18-128">Calendars.Read</span></span> | <span data-ttu-id="07c18-129">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="07c18-129">Calendars.Read</span></span> |
| [<span data-ttu-id="07c18-130">連絡先</span><span class="sxs-lookup"><span data-stu-id="07c18-130">contact</span></span>](../resources/contact.md) | <span data-ttu-id="07c18-131">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="07c18-131">Contacts.Read</span></span> | <span data-ttu-id="07c18-132">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="07c18-132">Contacts.Read</span></span> | <span data-ttu-id="07c18-133">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="07c18-133">Contacts.Read</span></span> |
| [<span data-ttu-id="07c18-134">contactFolder</span><span class="sxs-lookup"><span data-stu-id="07c18-134">contactFolder</span></span>](../resources/contactfolder.md) | <span data-ttu-id="07c18-135">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="07c18-135">Contacts.Read</span></span> | <span data-ttu-id="07c18-136">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="07c18-136">Contacts.Read</span></span> | <span data-ttu-id="07c18-137">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="07c18-137">Contacts.Read</span></span> |
| [<span data-ttu-id="07c18-138">event</span><span class="sxs-lookup"><span data-stu-id="07c18-138">event</span></span>](../resources/event.md) | <span data-ttu-id="07c18-139">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="07c18-139">Calendars.Read</span></span> | <span data-ttu-id="07c18-140">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="07c18-140">Calendars.Read</span></span> |  <span data-ttu-id="07c18-141">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="07c18-141">Calendars.Read</span></span>|
| <span data-ttu-id="07c18-142">グループ [calendar](../resources/calendar.md)</span><span class="sxs-lookup"><span data-stu-id="07c18-142">group [calendar](../resources/calendar.md)</span></span> | <span data-ttu-id="07c18-143">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="07c18-143">Group.Read.All</span></span> | <span data-ttu-id="07c18-144">非サポート</span><span class="sxs-lookup"><span data-stu-id="07c18-144">Not supported</span></span> | <span data-ttu-id="07c18-145">非サポート</span><span class="sxs-lookup"><span data-stu-id="07c18-145">Not supported</span></span> |
| <span data-ttu-id="07c18-146">グループ [event](../resources/event.md)</span><span class="sxs-lookup"><span data-stu-id="07c18-146">group [event](../resources/event.md)</span></span> | <span data-ttu-id="07c18-147">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="07c18-147">Group.Read.All</span></span> | <span data-ttu-id="07c18-148">非サポート</span><span class="sxs-lookup"><span data-stu-id="07c18-148">Not supported</span></span> | <span data-ttu-id="07c18-149">非サポート</span><span class="sxs-lookup"><span data-stu-id="07c18-149">Not supported</span></span> |
| <span data-ttu-id="07c18-150">グループ [post](../resources/post.md)</span><span class="sxs-lookup"><span data-stu-id="07c18-150">group [post](../resources/post.md)</span></span> | <span data-ttu-id="07c18-151">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="07c18-151">Group.Read.All</span></span> | <span data-ttu-id="07c18-152">サポート対象外</span><span class="sxs-lookup"><span data-stu-id="07c18-152">Not supported</span></span> | <span data-ttu-id="07c18-153">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="07c18-153">Group.Read.All</span></span> |
| [<span data-ttu-id="07c18-154">mailFolder</span><span class="sxs-lookup"><span data-stu-id="07c18-154">mailFolder</span></span>](../resources/mailfolder.md) | <span data-ttu-id="07c18-155">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="07c18-155">Mail.Read</span></span> | <span data-ttu-id="07c18-156">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="07c18-156">Mail.Read</span></span> | <span data-ttu-id="07c18-157">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="07c18-157">Mail.Read</span></span> |
| [<span data-ttu-id="07c18-158">message</span><span class="sxs-lookup"><span data-stu-id="07c18-158">message</span></span>](../resources/message.md) | <span data-ttu-id="07c18-159">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="07c18-159">Mail.Read</span></span> | <span data-ttu-id="07c18-160">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="07c18-160">Mail.Read</span></span> | <span data-ttu-id="07c18-161">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="07c18-161">Mail.Read</span></span> |
 
## <a name="http-request"></a><span data-ttu-id="07c18-162">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="07c18-162">HTTP request</span></span>

<span data-ttu-id="07c18-p103">**id** プロパティに対するフィルターと一致する拡張プロパティで展開された、リソース インスタンスを取得します。フィルター文字列内のスペース文字に [URL エンコード](https://www.w3schools.com/tags/ref_urlencode.asp)を適用していることを確認してください。</span><span class="sxs-lookup"><span data-stu-id="07c18-p103">Get a resource instance expanded with the extended property which matches a filter on the **id** property. Make sure you apply [URL encoding](https://www.w3schools.com/tags/ref_urlencode.asp) to the space characters in the filter string.</span></span>

<span data-ttu-id="07c18-165">**message** インスタンスの取得:</span><span class="sxs-lookup"><span data-stu-id="07c18-165">Get a **message** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/messages/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /me/mailFolders/{id}/messages/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="07c18-166">**mailFolder** インスタンスの取得:</span><span class="sxs-lookup"><span data-stu-id="07c18-166">Get a **mailFolder** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/mailFolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="07c18-167">**event** インスタンスの取得:</span><span class="sxs-lookup"><span data-stu-id="07c18-167">Get an **event** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/events/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/events/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="07c18-168">**calendar** インスタンスの取得:</span><span class="sxs-lookup"><span data-stu-id="07c18-168">Get a **calendar** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendars/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/calendars/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="07c18-169">**contact** インスタンスの取得:</span><span class="sxs-lookup"><span data-stu-id="07c18-169">Get a **contact** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contacts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /me/contactFolders/{id}/contacts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}/contacts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="07c18-170">**contactFolder** インスタンスの取得:</span><span class="sxs-lookup"><span data-stu-id="07c18-170">Get a **contactFolder** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contactfolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```
<span data-ttu-id="07c18-171">グループ **event** インスタンスの取得:</span><span class="sxs-lookup"><span data-stu-id="07c18-171">Get a group **event** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/events/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```

<span data-ttu-id="07c18-172">グループ **post** インスタンスの取得:</span><span class="sxs-lookup"><span data-stu-id="07c18-172">Get a group **post** instance:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}/posts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```

## <a name="path-parameters"></a><span data-ttu-id="07c18-173">パス パラメーター</span><span class="sxs-lookup"><span data-stu-id="07c18-173">Path parameters</span></span>
|<span data-ttu-id="07c18-174">パラメーター</span><span class="sxs-lookup"><span data-stu-id="07c18-174">Parameter</span></span>|<span data-ttu-id="07c18-175">型</span><span class="sxs-lookup"><span data-stu-id="07c18-175">Type</span></span>|<span data-ttu-id="07c18-176">説明</span><span class="sxs-lookup"><span data-stu-id="07c18-176">Description</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="07c18-177">id_value</span><span class="sxs-lookup"><span data-stu-id="07c18-177">id_value</span></span>|<span data-ttu-id="07c18-178">String</span><span class="sxs-lookup"><span data-stu-id="07c18-178">String</span></span>|<span data-ttu-id="07c18-p104">照合する拡張プロパティの ID。サポートされている形式のいずれかに従う必要があります。詳しくは、「[Outlook の拡張プロパティの概要](../resources/extended-properties-overview.md)」を参照してください。必須。</span><span class="sxs-lookup"><span data-stu-id="07c18-p104">The ID of the extended property to match. It must follow one of the supported formats. See [Outlook extended properties overview](../resources/extended-properties-overview.md) for more information. Required.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="07c18-183">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="07c18-183">Request headers</span></span>
| <span data-ttu-id="07c18-184">名前</span><span class="sxs-lookup"><span data-stu-id="07c18-184">Name</span></span>      |<span data-ttu-id="07c18-185">説明</span><span class="sxs-lookup"><span data-stu-id="07c18-185">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="07c18-186">Authorization</span><span class="sxs-lookup"><span data-stu-id="07c18-186">Authorization</span></span>  | <span data-ttu-id="07c18-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="07c18-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="07c18-189">要求本文</span><span class="sxs-lookup"><span data-stu-id="07c18-189">Request body</span></span>
<span data-ttu-id="07c18-190">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="07c18-190">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="07c18-191">応答</span><span class="sxs-lookup"><span data-stu-id="07c18-191">Response</span></span>

<span data-ttu-id="07c18-192">成功した場合、このメソッドは `200 OK` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="07c18-192">If successful, this method returns a `200 OK` response code.</span></span> 

<span data-ttu-id="07c18-193">応答本文には、一致する [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) オブジェクトで展開された、要求したリソース インスタンスで表されるオブジェクトが含まれます。</span><span class="sxs-lookup"><span data-stu-id="07c18-193">The response body includes an object representing the requested resource instance, expanded with the matching [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) object.</span></span>

## <a name="example"></a><span data-ttu-id="07c18-194">例</span><span class="sxs-lookup"><span data-stu-id="07c18-194">Example</span></span>
##### <a name="request"></a><span data-ttu-id="07c18-195">要求</span><span class="sxs-lookup"><span data-stu-id="07c18-195">Request</span></span>
<span data-ttu-id="07c18-p106">この例では、複数値の拡張プロパティを含めることで指定されたイベントを取得して展開します。フィルターは、**id** が文字列 `StringArray {66f5a359-4659-4830-9070-00050ec6ac6e} Name Recreation` と一致する拡張プロパティを返します (ここでは、読みやすくするため URL エンコードを削除しています)。</span><span class="sxs-lookup"><span data-stu-id="07c18-p106">This example gets and expands the specified event by including a multi-value extended property. The filter returns the extended property that has its **id** matching the string `StringArray {66f5a359-4659-4830-9070-00050ec6ac6e} Name Recreation` (with URL encoding removed here for ease of reading).</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/me/events('AAMkAGE1M2_bs88AACbuFiiAAA=')?$expand=multiValueExtendedProperties($filter=id%20eq%20'StringArray%20{66f5a359-4659-4830-9070-00050ec6ac6e}%20Name%20Recreation')
```
##### <a name="response"></a><span data-ttu-id="07c18-198">応答</span><span class="sxs-lookup"><span data-stu-id="07c18-198">Response</span></span>

<span data-ttu-id="07c18-199">応答本文には、指定されたイベントのすべてのプロパティと、フィルターから返される拡張プロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="07c18-199">The response body includes all the properties of the specified event and extended property returned from the filter.</span></span>

<span data-ttu-id="07c18-p107">注:簡潔にするために、ここに示す**イベント** オブジェクトは切り詰められています。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="07c18-p107">Note: The **event** object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>

<!-- { "blockType": "ignored" } -->
```http
HTTP/1.1 200 OK
Content-type: application/json
{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Me/events/$entity",
    "@odata.id": "https://graph.microsoft.com/v1.0/users('ddfcd489-628b-40d7-b48b-57002df800e5@1717622f-1d94-4d0c-9d74-709fad664b77')/events('AAMkAGE1M2_bs88AACbuFiiAAA=')",
    "@odata.etag": "W/\"mODEKWhc/Um6lA3uPm7PPAAAm8k15A==\"",
    "id": "AAMkAGE1M2_bs88AACbuFiiAAA=",
    "start": {
        "dateTime": "2015-11-26T17:00:00.0000000",
        "timeZone": "UTC"
    },
    "end": {
        "dateTime": "2015-11-30T05:00:00.0000000",
        "timeZone": "UTC"
    },
    "organizer": {
        "emailAddress": {
            "name": "Christine Irwin",
            "address": "christine@contoso.com"
        }
    },
    "multiValueExtendedProperties@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Me/events('AAMkAGE1M2_bs88AACbuFiiAAA%3D')/multiValueExtendedProperties",
    "multiValueExtendedProperties": [
        {
            "id": "StringArray {66f5a359-4659-4830-9070-00050ec6ac6e} Name Recreation",
            "value": [
                "Food",
                "Hiking",
                "Swimming"
            ]
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get multiValueLegacyExtendedProperty",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
