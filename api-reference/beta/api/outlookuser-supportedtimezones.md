---
title: 'outlookUser: supportedTimeZones'
description: ユーザーに対してサポートされている (ユーザーのメールボックス サーバーで構成されている) タイム ゾーンのリストを取得します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: f54457169b4f4f214488727fa94b7402b0f33724
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27963564"
---
# <a name="outlookuser-supportedtimezones"></a><span data-ttu-id="1f534-103">outlookUser: supportedTimeZones</span><span class="sxs-lookup"><span data-stu-id="1f534-103">outlookUser: supportedTimeZones</span></span>

> <span data-ttu-id="1f534-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="1f534-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1f534-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1f534-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1f534-106">ユーザーに対してサポートされている (ユーザーのメールボックス サーバーで構成されている) タイム ゾーンのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="1f534-106">Get the list of time zones that are supported for the user, as configured on the user's mailbox server.</span></span>

<span data-ttu-id="1f534-107">Windows のタイム ゾーン形式または [Internet Assigned Numbers Authority (IANA) のタイム ゾーン](https://www.iana.org/time-zones) (別称: Olson タイム ゾーン) 形式でタイム ゾーンが返されるよう、明示的に指定できます。</span><span class="sxs-lookup"><span data-stu-id="1f534-107">You can explicitly specify to have time zones returned in the Windows time zone format or  [Internet Assigned Numbers Authority (IANA) time zone](https://www.iana.org/time-zones) (also known as Olson time zone) format.</span></span> <span data-ttu-id="1f534-108">既定値は Windows 形式です。</span><span class="sxs-lookup"><span data-stu-id="1f534-108">The Windows format is the default.</span></span>

<span data-ttu-id="1f534-109">Outlook クライアントを設定する際は、このサポートされているリストから、優先するタイム ゾーンを選択します。</span><span class="sxs-lookup"><span data-stu-id="1f534-109">When setting up an Outlook client, the user selects the preferred time zone from this supported list.</span></span> <span data-ttu-id="1f534-110">これにより、[ユーザーのメールボックス設定を取得](user-get-mailboxsettings.md)することによって、優先タイム ゾーンを取得できるようになります。</span><span class="sxs-lookup"><span data-stu-id="1f534-110">You can subsequently get the preferred time zone by [getting the user's mailbox settings](user-get-mailboxsettings.md).</span></span>


## <a name="permissions"></a><span data-ttu-id="1f534-111">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="1f534-111">Permissions</span></span>
<span data-ttu-id="1f534-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1f534-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1f534-114">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1f534-114">Permission type</span></span>      | <span data-ttu-id="1f534-115">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="1f534-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1f534-116">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="1f534-116">Delegated (work or school account)</span></span> | <span data-ttu-id="1f534-117">User.Read、User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="1f534-117">User.Read, User.ReadBasic.All</span></span>    |
|<span data-ttu-id="1f534-118">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1f534-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1f534-119">User.Read</span><span class="sxs-lookup"><span data-stu-id="1f534-119">User.Read</span></span>    |
|<span data-ttu-id="1f534-120">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1f534-120">Application</span></span> | <span data-ttu-id="1f534-121">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="1f534-121">User.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1f534-122">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1f534-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/supportedTimeZones
GET /users/{id|userPrincipalName}/outlook/supportedTimeZones

GET /me/outlook/supportedTimeZones(TimeZoneStandard=microsoft.graph.timeZoneStandard'{timezone_format}')
GET /users/{id|userPrincipalName}/outlook/supportedTimeZones(TimeZoneStandard=microsoft.graph.timeZoneStandard'{timezone_format}')
```

## <a name="function-parameters"></a><span data-ttu-id="1f534-123">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="1f534-123">Function parameters</span></span>
| <span data-ttu-id="1f534-124">パラメーター</span><span class="sxs-lookup"><span data-stu-id="1f534-124">Parameter</span></span>      | <span data-ttu-id="1f534-125">型</span><span class="sxs-lookup"><span data-stu-id="1f534-125">Type</span></span>    | <span data-ttu-id="1f534-126">説明</span><span class="sxs-lookup"><span data-stu-id="1f534-126">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="1f534-127">TimeZoneStandard</span><span class="sxs-lookup"><span data-stu-id="1f534-127">TimeZoneStandard</span></span>  | <span data-ttu-id="1f534-128">String</span><span class="sxs-lookup"><span data-stu-id="1f534-128">String</span></span>  | <span data-ttu-id="1f534-129">タイム ゾーンの形式。</span><span class="sxs-lookup"><span data-stu-id="1f534-129">A time zone format.</span></span> <span data-ttu-id="1f534-130">サポートされている値は `Windows` および `Iana` です。</span><span class="sxs-lookup"><span data-stu-id="1f534-130">Supported values are: `Windows`, and `Iana`.</span></span> <span data-ttu-id="1f534-131">省略可能。</span><span class="sxs-lookup"><span data-stu-id="1f534-131">Optional.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="1f534-132">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1f534-132">Request headers</span></span>
| <span data-ttu-id="1f534-133">名前</span><span class="sxs-lookup"><span data-stu-id="1f534-133">Name</span></span>       | <span data-ttu-id="1f534-134">型</span><span class="sxs-lookup"><span data-stu-id="1f534-134">Type</span></span> | <span data-ttu-id="1f534-135">説明</span><span class="sxs-lookup"><span data-stu-id="1f534-135">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="1f534-136">Authorization</span><span class="sxs-lookup"><span data-stu-id="1f534-136">Authorization</span></span>  | <span data-ttu-id="1f534-137">string</span><span class="sxs-lookup"><span data-stu-id="1f534-137">string</span></span>  | <span data-ttu-id="1f534-p106">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="1f534-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1f534-140">要求本文</span><span class="sxs-lookup"><span data-stu-id="1f534-140">Request body</span></span>
<span data-ttu-id="1f534-141">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="1f534-141">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1f534-142">応答</span><span class="sxs-lookup"><span data-stu-id="1f534-142">Response</span></span>
<span data-ttu-id="1f534-143">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文に [timeZoneInformation](../resources/timezoneinformation.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="1f534-143">If successful, this method returns `200 OK` response code and a collection of [timeZoneInformation](../resources/timezoneinformation.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1f534-144">例</span><span class="sxs-lookup"><span data-stu-id="1f534-144">Example</span></span>

##### <a name="request-1"></a><span data-ttu-id="1f534-145">要求 1</span><span class="sxs-lookup"><span data-stu-id="1f534-145">Request 1</span></span>
<span data-ttu-id="1f534-146">次の例では、`timeZoneStandard` パラメーターを指定せずに、Windows のタイム ゾーン形式で表記されたサポート対象タイム ゾーンのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="1f534-146">The following example does not specify the `timeZoneStandard` parameter, and gets the list of supported time zones represented in the Windows time zone format.</span></span> 
<!-- {
  "blockType": "request",
  "name": "user_supportedtimezones_default"
}-->
```http
GET https://graph.microsoft.com/beta/me/outlook/supportedTimeZones
```

##### <a name="response-1"></a><span data-ttu-id="1f534-147">応答 1</span><span class="sxs-lookup"><span data-stu-id="1f534-147">Response 1</span></span>
<span data-ttu-id="1f534-148">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="1f534-148">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "name": "user_supportedtimezones_default",
  "truncated": true,
  "@odata.type": "microsoft.graph.timeZoneInformation",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.timeZoneInformation)",
  "value":[
    {
      "alias":"Dateline Standard Time",
      "displayName":"(UTC-12:00) International Date Line West"
    },
    {
      "alias":"Samoa Standard Time",
      "displayName":"(UTC+13:00) Samoa"
    },
    {
       "alias":"UTC-11",
       "displayName":"(UTC-11:00) Coordinated Universal Time-11"
    },
    {
      "alias":"Aleutian Standard Time",
      "displayName":"(UTC-10:00) Aleutian Islands"
    }
  ]
}
```

##### <a name="request-2"></a><span data-ttu-id="1f534-149">要求 2</span><span class="sxs-lookup"><span data-stu-id="1f534-149">Request 2</span></span>
<span data-ttu-id="1f534-150">次の例では、`TimeZoneStandard` パラメーターに `Iana` を指定して、IANA 形式で表記されたサポート対象タイム ゾーンのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="1f534-150">The following example specifies `Iana` for the `TimeZoneStandard` parameter, and gets the list of supported time zones represented in IANA format.</span></span> 

<!-- {
  "blockType": "request",
  "name": "user_supportedtimezones_iana"
} -->

```http
GET https://graph.microsoft.com/beta/me/outlook/supportedTimeZones(TimeZoneStandard=microsoft.graph.timeZoneStandard'Iana')
```

##### <a name="response-2"></a><span data-ttu-id="1f534-151">応答 2</span><span class="sxs-lookup"><span data-stu-id="1f534-151">Response 2</span></span>
<span data-ttu-id="1f534-152">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="1f534-152">Here is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "name": "user_supportedtimezones_iana",
  "truncated": true,
  "@odata.type": "microsoft.graph.timeZoneInformation",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.timeZoneInformation)",
  "value":[
    {
      "alias":"Etc/GMT+12",
      "displayName":"Etc/GMT+12"
    },
    {
      "alias":"US/Samoa",
      "displayName":"US/Samoa"
    },
    {
      "alias":"Etc/GMT+11",
      "displayName":"Etc/GMT+11"
    },
    {
      "alias":"US/Aleutian",
      "displayName":"US/Aleutian"
    }
  ]
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user: supportedTimeZones",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
