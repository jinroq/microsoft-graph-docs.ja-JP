---
title: audioconferencing リソースの種類
description: onlineMeeting の電話アクセス情報を表します。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 1371e80830bf148588f6bda91326b0521fcdda42
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33328375"
---
# <a name="audioconferencing-resource-type"></a><span data-ttu-id="0df13-103">audioconferencing リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0df13-103">audioConferencing resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0df13-104">[onlineMeeting](onlinemeeting.md)の電話アクセス情報を表します。</span><span class="sxs-lookup"><span data-stu-id="0df13-104">Represents phone access information for an [onlineMeeting](onlinemeeting.md).</span></span>

## <a name="properties"></a><span data-ttu-id="0df13-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0df13-105">Properties</span></span>

| <span data-ttu-id="0df13-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0df13-106">Property</span></span>            | <span data-ttu-id="0df13-107">型</span><span class="sxs-lookup"><span data-stu-id="0df13-107">Type</span></span>    | <span data-ttu-id="0df13-108">説明</span><span class="sxs-lookup"><span data-stu-id="0df13-108">Description</span></span>                                                                    |
|:--------------------|:--------|:-------------------------------------------------------------------------------|
| <span data-ttu-id="0df13-109">ダイヤルイン url</span><span class="sxs-lookup"><span data-stu-id="0df13-109">dialinUrl</span></span>           | <span data-ttu-id="0df13-110">String</span><span class="sxs-lookup"><span data-stu-id="0df13-110">String</span></span>  | <span data-ttu-id="0df13-111">外部からアクセス可能な web ページへの URL。ダイヤルイン情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="0df13-111">A URL to the externally-accessible web page that contains dial-in information.</span></span> |
| <span data-ttu-id="0df13-112">leaderPasscode</span><span class="sxs-lookup"><span data-stu-id="0df13-112">leaderPasscode</span></span>      | <span data-ttu-id="0df13-113">String</span><span class="sxs-lookup"><span data-stu-id="0df13-113">String</span></span>  | <span data-ttu-id="0df13-114">電話会議プロバイダーに接続するために必要なリーダーパスワード。</span><span class="sxs-lookup"><span data-stu-id="0df13-114">The leader password required to connect to the Audio Conference Provider.</span></span>      |
| <span data-ttu-id="0df13-115">participantPasscode</span><span class="sxs-lookup"><span data-stu-id="0df13-115">participantPasscode</span></span> | <span data-ttu-id="0df13-116">String</span><span class="sxs-lookup"><span data-stu-id="0df13-116">String</span></span>  | <span data-ttu-id="0df13-117">音声会議プロバイダーに接続するために必要な、参加者のパスワード。</span><span class="sxs-lookup"><span data-stu-id="0df13-117">The participant password required to connect to the Audio Conference Provider.</span></span> |
| <span data-ttu-id="0df13-118">tollFreeNumber</span><span class="sxs-lookup"><span data-stu-id="0df13-118">tollFreeNumber</span></span>      | <span data-ttu-id="0df13-119">String</span><span class="sxs-lookup"><span data-stu-id="0df13-119">String</span></span>  | <span data-ttu-id="0df13-120">音声会議プロバイダーに接続するための無料電話番号。</span><span class="sxs-lookup"><span data-stu-id="0df13-120">The toll-free number to connect to the Audio Conference Provider.</span></span>              |
| <span data-ttu-id="0df13-121">tollNumber</span><span class="sxs-lookup"><span data-stu-id="0df13-121">tollNumber</span></span>          | <span data-ttu-id="0df13-122">String</span><span class="sxs-lookup"><span data-stu-id="0df13-122">String</span></span>  | <span data-ttu-id="0df13-123">音声会議プロバイダーに接続する有料電話番号。</span><span class="sxs-lookup"><span data-stu-id="0df13-123">The toll number to connect to the Audio Conference Provider.</span></span>                   |

## <a name="json-representation"></a><span data-ttu-id="0df13-124">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0df13-124">JSON representation</span></span>

<span data-ttu-id="0df13-125">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="0df13-125">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "audioConferencing resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
