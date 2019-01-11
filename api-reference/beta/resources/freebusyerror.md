---
title: freeBusyError リソースの種類
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。"
localization_priority: Normal
ms.openlocfilehash: 63cfc4b14ba6176d582155df57b7f7f787e63cf4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27889769"
---
# <a name="freebusyerror-resource-type"></a><span data-ttu-id="d0413-104">freeBusyError リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d0413-104">freeBusyError resource type</span></span>

 > <span data-ttu-id="d0413-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="d0413-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d0413-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d0413-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="d0413-107">ユーザー、配布リスト、またはリソースの可用性を取得しようとしていますからエラー情報を表します。</span><span class="sxs-lookup"><span data-stu-id="d0413-107">Represents error information from attempting to get the availability of a user, distribution list, or resource.</span></span>

## <a name="properties"></a><span data-ttu-id="d0413-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d0413-108">Properties</span></span>
| <span data-ttu-id="d0413-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d0413-109">Property</span></span>     | <span data-ttu-id="d0413-110">種類</span><span class="sxs-lookup"><span data-stu-id="d0413-110">Type</span></span>   |<span data-ttu-id="d0413-111">説明</span><span class="sxs-lookup"><span data-stu-id="d0413-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d0413-112">message</span><span class="sxs-lookup"><span data-stu-id="d0413-112">message</span></span> |<span data-ttu-id="d0413-113">String</span><span class="sxs-lookup"><span data-stu-id="d0413-113">String</span></span> |<span data-ttu-id="d0413-114">エラーをについて説明します。</span><span class="sxs-lookup"><span data-stu-id="d0413-114">Describes the error.</span></span> |
|<span data-ttu-id="d0413-115">responseCode</span><span class="sxs-lookup"><span data-stu-id="d0413-115">responseCode</span></span> |<span data-ttu-id="d0413-116">String</span><span class="sxs-lookup"><span data-stu-id="d0413-116">String</span></span> |<span data-ttu-id="d0413-117">ユーザー、配布リスト、またはリソースの可用性のクエリからの応答コード。</span><span class="sxs-lookup"><span data-stu-id="d0413-117">The response code from querying for the availability of the user, distribution list, or resource.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="d0413-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d0413-118">JSON representation</span></span>

<span data-ttu-id="d0413-119">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d0413-119">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.freeBusyError"
}-->

```json
{
  "message": "String",
  "responseCode": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "freeBusyError resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
