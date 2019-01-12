---
title: audioConferencing リソースの種類
description: OnlineMeeting には、電話アクセス情報を表します。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: cd65b094a17ad3fa470471c3ed6dd3908367e578
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27977508"
---
# <a name="audioconferencing-resource-type"></a><span data-ttu-id="1d4e1-103">audioConferencing リソースの種類</span><span class="sxs-lookup"><span data-stu-id="1d4e1-103">audioConferencing resource type</span></span>

> <span data-ttu-id="1d4e1-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="1d4e1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1d4e1-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1d4e1-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1d4e1-106">[OnlineMeeting](onlinemeeting.md)には、電話アクセス情報を表します。</span><span class="sxs-lookup"><span data-stu-id="1d4e1-106">Represents phone access information for an [onlineMeeting](onlinemeeting.md).</span></span>

## <a name="properties"></a><span data-ttu-id="1d4e1-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1d4e1-107">Properties</span></span>

| <span data-ttu-id="1d4e1-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1d4e1-108">Property</span></span>            | <span data-ttu-id="1d4e1-109">種類</span><span class="sxs-lookup"><span data-stu-id="1d4e1-109">Type</span></span>    | <span data-ttu-id="1d4e1-110">説明</span><span class="sxs-lookup"><span data-stu-id="1d4e1-110">Description</span></span>                                                                    |
|:--------------------|:--------|:-------------------------------------------------------------------------------|
| <span data-ttu-id="1d4e1-111">dialinUrl</span><span class="sxs-lookup"><span data-stu-id="1d4e1-111">dialinUrl</span></span>           | <span data-ttu-id="1d4e1-112">String</span><span class="sxs-lookup"><span data-stu-id="1d4e1-112">String</span></span>  | <span data-ttu-id="1d4e1-113">ダイヤルイン情報を含む外部からアクセス可能な web ページの URL です。</span><span class="sxs-lookup"><span data-stu-id="1d4e1-113">A URL to the externally-accessible web page that contains dial-in information.</span></span> |
| <span data-ttu-id="1d4e1-114">leaderPasscode</span><span class="sxs-lookup"><span data-stu-id="1d4e1-114">leaderPasscode</span></span>      | <span data-ttu-id="1d4e1-115">String</span><span class="sxs-lookup"><span data-stu-id="1d4e1-115">String</span></span>  | <span data-ttu-id="1d4e1-116">オーディオ会議プロバイダーへの接続に必要なリーダーのパスワードです。</span><span class="sxs-lookup"><span data-stu-id="1d4e1-116">The leader password required to connect to the Audio Conference Provider.</span></span>      |
| <span data-ttu-id="1d4e1-117">participantPasscode</span><span class="sxs-lookup"><span data-stu-id="1d4e1-117">participantPasscode</span></span> | <span data-ttu-id="1d4e1-118">String</span><span class="sxs-lookup"><span data-stu-id="1d4e1-118">String</span></span>  | <span data-ttu-id="1d4e1-119">オーディオ会議プロバイダーへの接続に必要な参加者のパスワードです。</span><span class="sxs-lookup"><span data-stu-id="1d4e1-119">The participant password required to connect to the Audio Conference Provider.</span></span> |
| <span data-ttu-id="1d4e1-120">tollFreeNumber</span><span class="sxs-lookup"><span data-stu-id="1d4e1-120">tollFreeNumber</span></span>      | <span data-ttu-id="1d4e1-121">String</span><span class="sxs-lookup"><span data-stu-id="1d4e1-121">String</span></span>  | <span data-ttu-id="1d4e1-122">オーディオ会議プロバイダーに接続する無料電話番号です。</span><span class="sxs-lookup"><span data-stu-id="1d4e1-122">The toll-free number to connect to the Audio Conference Provider.</span></span>              |
| <span data-ttu-id="1d4e1-123">tollNumber</span><span class="sxs-lookup"><span data-stu-id="1d4e1-123">tollNumber</span></span>          | <span data-ttu-id="1d4e1-124">String</span><span class="sxs-lookup"><span data-stu-id="1d4e1-124">String</span></span>  | <span data-ttu-id="1d4e1-125">オーディオ会議プロバイダーに接続する有料電話番号です。</span><span class="sxs-lookup"><span data-stu-id="1d4e1-125">The toll number to connect to the Audio Conference Provider.</span></span>                   |

## <a name="json-representation"></a><span data-ttu-id="1d4e1-126">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="1d4e1-126">JSON representation</span></span>

<span data-ttu-id="1d4e1-127">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="1d4e1-127">The following is a JSON representation of the resource.</span></span>

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
