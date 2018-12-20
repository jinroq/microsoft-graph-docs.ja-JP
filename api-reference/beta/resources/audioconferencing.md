---
title: audioConferencing リソースの種類
description: OnlineMeeting には、電話アクセス情報を表します。
author: VinodRavichandran
ms.openlocfilehash: 4e2ee26e6f9a86d50efcb21cd95b84b207488ef1
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380227"
---
# <a name="audioconferencing-resource-type"></a><span data-ttu-id="8ffb8-103">audioConferencing リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8ffb8-103">audioConferencing resource type</span></span>

> <span data-ttu-id="8ffb8-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="8ffb8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8ffb8-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8ffb8-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8ffb8-106">[OnlineMeeting](onlinemeeting.md)には、電話アクセス情報を表します。</span><span class="sxs-lookup"><span data-stu-id="8ffb8-106">Represents phone access information for an [onlineMeeting](onlinemeeting.md).</span></span>

## <a name="properties"></a><span data-ttu-id="8ffb8-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8ffb8-107">Properties</span></span>

| <span data-ttu-id="8ffb8-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8ffb8-108">Property</span></span>            | <span data-ttu-id="8ffb8-109">型</span><span class="sxs-lookup"><span data-stu-id="8ffb8-109">Type</span></span>    | <span data-ttu-id="8ffb8-110">説明</span><span class="sxs-lookup"><span data-stu-id="8ffb8-110">Description</span></span>                                                                    |
|:--------------------|:--------|:-------------------------------------------------------------------------------|
| <span data-ttu-id="8ffb8-111">dialinUrl</span><span class="sxs-lookup"><span data-stu-id="8ffb8-111">dialinUrl</span></span>           | <span data-ttu-id="8ffb8-112">String</span><span class="sxs-lookup"><span data-stu-id="8ffb8-112">String</span></span>  | <span data-ttu-id="8ffb8-113">ダイヤルイン情報を含む外部からアクセス可能な web ページの URL です。</span><span class="sxs-lookup"><span data-stu-id="8ffb8-113">A URL to the externally-accessible web page that contains dial-in information.</span></span> |
| <span data-ttu-id="8ffb8-114">leaderPasscode</span><span class="sxs-lookup"><span data-stu-id="8ffb8-114">leaderPasscode</span></span>      | <span data-ttu-id="8ffb8-115">String</span><span class="sxs-lookup"><span data-stu-id="8ffb8-115">String</span></span>  | <span data-ttu-id="8ffb8-116">オーディオ会議プロバイダーへの接続に必要なリーダーのパスワードです。</span><span class="sxs-lookup"><span data-stu-id="8ffb8-116">The leader password required to connect to the Audio Conference Provider.</span></span>      |
| <span data-ttu-id="8ffb8-117">participantPasscode</span><span class="sxs-lookup"><span data-stu-id="8ffb8-117">participantPasscode</span></span> | <span data-ttu-id="8ffb8-118">String</span><span class="sxs-lookup"><span data-stu-id="8ffb8-118">String</span></span>  | <span data-ttu-id="8ffb8-119">オーディオ会議プロバイダーへの接続に必要な参加者のパスワードです。</span><span class="sxs-lookup"><span data-stu-id="8ffb8-119">The participant password required to connect to the Audio Conference Provider.</span></span> |
| <span data-ttu-id="8ffb8-120">tollFreeNumber</span><span class="sxs-lookup"><span data-stu-id="8ffb8-120">tollFreeNumber</span></span>      | <span data-ttu-id="8ffb8-121">String</span><span class="sxs-lookup"><span data-stu-id="8ffb8-121">String</span></span>  | <span data-ttu-id="8ffb8-122">オーディオ会議プロバイダーに接続する無料電話番号です。</span><span class="sxs-lookup"><span data-stu-id="8ffb8-122">The toll-free number to connect to the Audio Conference Provider.</span></span>              |
| <span data-ttu-id="8ffb8-123">tollNumber</span><span class="sxs-lookup"><span data-stu-id="8ffb8-123">tollNumber</span></span>          | <span data-ttu-id="8ffb8-124">String</span><span class="sxs-lookup"><span data-stu-id="8ffb8-124">String</span></span>  | <span data-ttu-id="8ffb8-125">オーディオ会議プロバイダーに接続する有料電話番号です。</span><span class="sxs-lookup"><span data-stu-id="8ffb8-125">The toll number to connect to the Audio Conference Provider.</span></span>                   |

## <a name="json-representation"></a><span data-ttu-id="8ffb8-126">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8ffb8-126">JSON representation</span></span>

<span data-ttu-id="8ffb8-127">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="8ffb8-127">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.audioConferencing"
}-->
```json
{
  "dialinUrl": "String",
  "leaderPasscode": "String",
  "participantPasscode": "String",
  "tollFreeNumber": "String",
  "tollNumber": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "audioConferencing resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
