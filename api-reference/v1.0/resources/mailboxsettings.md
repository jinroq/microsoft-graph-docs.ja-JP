---
title: mailboxSettings リソースの種類
description: サインイン ユーザーのプライマリ メールボックスの設定。
localization_priority: Normal
ms.openlocfilehash: d4df71930a26c711c59f164aca5090bda809b503
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27827000"
---
# <a name="mailboxsettings-resource-type"></a><span data-ttu-id="3dd28-103">mailboxSettings リソースの種類</span><span class="sxs-lookup"><span data-stu-id="3dd28-103">mailboxSettings resource type</span></span>

<span data-ttu-id="3dd28-104">サインイン ユーザーのプライマリ メールボックスの設定。</span><span class="sxs-lookup"><span data-stu-id="3dd28-104">Settings for the primary mailbox of the signed-in user.</span></span>


## <a name="properties"></a><span data-ttu-id="3dd28-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3dd28-105">Properties</span></span>
| <span data-ttu-id="3dd28-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3dd28-106">Property</span></span>     | <span data-ttu-id="3dd28-107">種類</span><span class="sxs-lookup"><span data-stu-id="3dd28-107">Type</span></span>   |<span data-ttu-id="3dd28-108">説明</span><span class="sxs-lookup"><span data-stu-id="3dd28-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3dd28-109">archiveFolder</span><span class="sxs-lookup"><span data-stu-id="3dd28-109">archiveFolder</span></span>|<span data-ttu-id="3dd28-110">文字列</span><span class="sxs-lookup"><span data-stu-id="3dd28-110">string</span></span>|<span data-ttu-id="3dd28-111">ユーザーのアーカイブ フォルダーのフォルダー ID。</span><span class="sxs-lookup"><span data-stu-id="3dd28-111">Folder ID of an archive folder for the user.</span></span>|
|<span data-ttu-id="3dd28-112">automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="3dd28-112">automaticRepliesSetting</span></span>|[<span data-ttu-id="3dd28-113">automaticRepliesSetting</span><span class="sxs-lookup"><span data-stu-id="3dd28-113">automaticRepliesSetting</span></span>](automaticrepliessetting.md)|<span data-ttu-id="3dd28-114">サインイン ユーザーからのメッセージを使用して、着信メールの送信者に自動的に通知する構成設定。</span><span class="sxs-lookup"><span data-stu-id="3dd28-114">Configuration settings to automatically notify the sender of an incoming email with a message from the signed-in user.</span></span>|
|<span data-ttu-id="3dd28-115">language</span><span class="sxs-lookup"><span data-stu-id="3dd28-115">language</span></span>|[<span data-ttu-id="3dd28-116">localeInfo</span><span class="sxs-lookup"><span data-stu-id="3dd28-116">localeInfo</span></span>](localeinfo.md)|<span data-ttu-id="3dd28-117">優先言語および国/地域を含むユーザーのロケール情報。</span><span class="sxs-lookup"><span data-stu-id="3dd28-117">The locale information for the user, including the preferred language and country/region.</span></span>|
|<span data-ttu-id="3dd28-118">timeZone</span><span class="sxs-lookup"><span data-stu-id="3dd28-118">timeZone</span></span>|<span data-ttu-id="3dd28-119">文字列</span><span class="sxs-lookup"><span data-stu-id="3dd28-119">string</span></span>|<span data-ttu-id="3dd28-120">ユーザーのメールボックスの既定のタイム ゾーン。</span><span class="sxs-lookup"><span data-stu-id="3dd28-120">The default time zone for the user's mailbox.</span></span>|
|<span data-ttu-id="3dd28-121">workingHours</span><span class="sxs-lookup"><span data-stu-id="3dd28-121">workingHours</span></span>|[<span data-ttu-id="3dd28-122">workingHours</span><span class="sxs-lookup"><span data-stu-id="3dd28-122">workingHours</span></span>](workinghours.md)|<span data-ttu-id="3dd28-123">ユーザーが働く曜日と、特定のタイムゾーンの時間。</span><span class="sxs-lookup"><span data-stu-id="3dd28-123">The days of the week and hours in a specific time zone that the user works.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3dd28-124">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="3dd28-124">JSON representation</span></span>

<span data-ttu-id="3dd28-125">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="3dd28-125">Here is a JSON representation of the resource.</span></span>

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
