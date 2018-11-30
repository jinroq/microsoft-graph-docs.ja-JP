---
title: mailboxSettings リソースの種類
description: サインイン ユーザーのプライマリ メールボックスの設定。
ms.openlocfilehash: 79a01c59ec0a891c13107095a950a7cc8ae0b547
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27066543"
---
# <a name="mailboxsettings-resource-type"></a><span data-ttu-id="aa421-103">mailboxSettings リソースの種類</span><span class="sxs-lookup"><span data-stu-id="aa421-103">mailboxSettings resource type</span></span>

> <span data-ttu-id="aa421-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="aa421-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="aa421-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="aa421-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="aa421-106">サインイン ユーザーのプライマリ メールボックスの設定。</span><span class="sxs-lookup"><span data-stu-id="aa421-106">Settings for the primary mailbox of the signed-in user.</span></span>


## <a name="properties"></a><span data-ttu-id="aa421-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="aa421-107">Properties</span></span>
| <span data-ttu-id="aa421-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="aa421-108">Property</span></span>     | <span data-ttu-id="aa421-109">型</span><span class="sxs-lookup"><span data-stu-id="aa421-109">Type</span></span>   |<span data-ttu-id="aa421-110">説明</span><span class="sxs-lookup"><span data-stu-id="aa421-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="aa421-111">archiveFolder</span><span class="sxs-lookup"><span data-stu-id="aa421-111">archiveFolder</span></span>|<span data-ttu-id="aa421-112">文字列</span><span class="sxs-lookup"><span data-stu-id="aa421-112">string</span></span>|<span data-ttu-id="aa421-113">ユーザーのアーカイブ フォルダーのフォルダー ID。</span><span class="sxs-lookup"><span data-stu-id="aa421-113">Folder ID of an archive folder for the user.</span></span>|
|<span data-ttu-id="aa421-114">automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="aa421-114">automaticRepliesSetting</span></span>|[<span data-ttu-id="aa421-115">automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="aa421-115">automaticRepliesSetting</span></span>](automaticrepliessetting.md)|<span data-ttu-id="aa421-116">サインイン ユーザーからのメッセージを使用して、着信メールの送信者に自動的に通知する構成設定。</span><span class="sxs-lookup"><span data-stu-id="aa421-116">Configuration settings to automatically notify the sender of an incoming email with a message from the signed-in user.</span></span>|
|<span data-ttu-id="aa421-117">language</span><span class="sxs-lookup"><span data-stu-id="aa421-117">language</span></span>|[<span data-ttu-id="aa421-118">localeInfo</span><span class="sxs-lookup"><span data-stu-id="aa421-118">localeInfo</span></span>](localeinfo.md)|<span data-ttu-id="aa421-119">優先言語および国/地域を含むユーザーのロケール情報。</span><span class="sxs-lookup"><span data-stu-id="aa421-119">The locale information for the user, including the preferred language and country/region.</span></span>|
|<span data-ttu-id="aa421-120">timeZone</span><span class="sxs-lookup"><span data-stu-id="aa421-120">timeZone</span></span>|<span data-ttu-id="aa421-121">文字列</span><span class="sxs-lookup"><span data-stu-id="aa421-121">string</span></span>|<span data-ttu-id="aa421-122">ユーザーのメールボックスの既定のタイム ゾーン。</span><span class="sxs-lookup"><span data-stu-id="aa421-122">The default time zone for the user's mailbox.</span></span>|
|<span data-ttu-id="aa421-123">workingHours</span><span class="sxs-lookup"><span data-stu-id="aa421-123">workingHours</span></span>|[<span data-ttu-id="aa421-124">workingHours</span><span class="sxs-lookup"><span data-stu-id="aa421-124">workingHours</span></span>](workinghours.md)|<span data-ttu-id="aa421-125">ユーザーが働く曜日と、特定のタイムゾーンの時間。</span><span class="sxs-lookup"><span data-stu-id="aa421-125">The days of the week and hours in a specific time zone that the user works.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="aa421-126">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="aa421-126">JSON representation</span></span>

<span data-ttu-id="aa421-127">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="aa421-127">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "archiveFolder"
  ],
  "@odata.type": "microsoft.graph.mailboxSettings"
}-->

```json
{
  "archiveFolder": "string",
  "automaticRepliesSetting": {"@odata.type": "microsoft.graph.automaticRepliesSetting"},
  "language": {"@odata.type": "microsoft.graph.localeInfo"},
  "timeZone": "string",
  "workingHours": {"@odata.type": "microsoft.graph.workingHours"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "mailboxSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->