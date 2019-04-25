---
title: audioconferencing リソースの種類
description: onlineMeeting の電話アクセス情報を表します。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: cb822f2049d84f9a2460370f05d5dfc85c347f15
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32535562"
---
# <a name="audioconferencing-resource-type"></a><span data-ttu-id="6031e-103">audioconferencing リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6031e-103">audioConferencing resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6031e-104">[onlineMeeting](onlinemeeting.md)の電話アクセス情報を表します。</span><span class="sxs-lookup"><span data-stu-id="6031e-104">Represents phone access information for an [onlineMeeting](onlinemeeting.md).</span></span>

## <a name="properties"></a><span data-ttu-id="6031e-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6031e-105">Properties</span></span>

| <span data-ttu-id="6031e-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6031e-106">Property</span></span>            | <span data-ttu-id="6031e-107">型</span><span class="sxs-lookup"><span data-stu-id="6031e-107">Type</span></span>    | <span data-ttu-id="6031e-108">説明</span><span class="sxs-lookup"><span data-stu-id="6031e-108">Description</span></span>                                                                    |
|:--------------------|:--------|:-------------------------------------------------------------------------------|
| <span data-ttu-id="6031e-109">ダイヤルイン url</span><span class="sxs-lookup"><span data-stu-id="6031e-109">dialinUrl</span></span>           | <span data-ttu-id="6031e-110">String</span><span class="sxs-lookup"><span data-stu-id="6031e-110">String</span></span>  | <span data-ttu-id="6031e-111">外部からアクセス可能な web ページへの URL。ダイヤルイン情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="6031e-111">A URL to the externally-accessible web page that contains dial-in information.</span></span> |
| <span data-ttu-id="6031e-112">leaderPasscode</span><span class="sxs-lookup"><span data-stu-id="6031e-112">leaderPasscode</span></span>      | <span data-ttu-id="6031e-113">String</span><span class="sxs-lookup"><span data-stu-id="6031e-113">String</span></span>  | <span data-ttu-id="6031e-114">電話会議プロバイダーに接続するために必要なリーダーパスワード。</span><span class="sxs-lookup"><span data-stu-id="6031e-114">The leader password required to connect to the Audio Conference Provider.</span></span>      |
| <span data-ttu-id="6031e-115">participantPasscode</span><span class="sxs-lookup"><span data-stu-id="6031e-115">participantPasscode</span></span> | <span data-ttu-id="6031e-116">String</span><span class="sxs-lookup"><span data-stu-id="6031e-116">String</span></span>  | <span data-ttu-id="6031e-117">音声会議プロバイダーに接続するために必要な、参加者のパスワード。</span><span class="sxs-lookup"><span data-stu-id="6031e-117">The participant password required to connect to the Audio Conference Provider.</span></span> |
| <span data-ttu-id="6031e-118">tollFreeNumber</span><span class="sxs-lookup"><span data-stu-id="6031e-118">tollFreeNumber</span></span>      | <span data-ttu-id="6031e-119">String</span><span class="sxs-lookup"><span data-stu-id="6031e-119">String</span></span>  | <span data-ttu-id="6031e-120">音声会議プロバイダーに接続するための無料電話番号。</span><span class="sxs-lookup"><span data-stu-id="6031e-120">The toll-free number to connect to the Audio Conference Provider.</span></span>              |
| <span data-ttu-id="6031e-121">tollNumber</span><span class="sxs-lookup"><span data-stu-id="6031e-121">tollNumber</span></span>          | <span data-ttu-id="6031e-122">String</span><span class="sxs-lookup"><span data-stu-id="6031e-122">String</span></span>  | <span data-ttu-id="6031e-123">音声会議プロバイダーに接続する有料電話番号。</span><span class="sxs-lookup"><span data-stu-id="6031e-123">The toll number to connect to the Audio Conference Provider.</span></span>                   |

## <a name="json-representation"></a><span data-ttu-id="6031e-124">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6031e-124">JSON representation</span></span>

<span data-ttu-id="6031e-125">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="6031e-125">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/audioconferencing.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
