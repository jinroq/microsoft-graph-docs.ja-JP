---
title: synchronizationJobRestartCriteria リソースの種類
description: 同期ジョブの範囲を定義し[ます。再起動](../api/synchronization_synchronizationjob_restart.md)アクション。
localization_priority: Normal
doc_type: resourcePageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 8fb363b74f1daff678d0751aca4a9033b01d9832
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964656"
---
# <a name="synchronizationjobrestartcriteria-resource-type"></a><span data-ttu-id="c5259-103">synchronizationJobRestartCriteria リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c5259-103">synchronizationJobRestartCriteria resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c5259-104">同期ジョブの範囲を定義し[ます。再起動](../api/synchronization-synchronizationjob-restart.md)アクション。</span><span class="sxs-lookup"><span data-stu-id="c5259-104">Defines the scope of the [synchronizationJob: restart](../api/synchronization-synchronizationjob-restart.md) action.</span></span>

## <a name="properties"></a><span data-ttu-id="c5259-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c5259-105">Properties</span></span>
| <span data-ttu-id="c5259-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c5259-106">Property</span></span>     | <span data-ttu-id="c5259-107">型</span><span class="sxs-lookup"><span data-stu-id="c5259-107">Type</span></span>   |<span data-ttu-id="c5259-108">説明</span><span class="sxs-lookup"><span data-stu-id="c5259-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c5259-109">resetScope</span><span class="sxs-lookup"><span data-stu-id="c5259-109">resetScope</span></span>|<span data-ttu-id="c5259-110">String</span><span class="sxs-lookup"><span data-stu-id="c5259-110">String</span></span>| <span data-ttu-id="c5259-111">`Full`、 `Watermark` `Escrows`、、、、 `ConnectorDataStore`の各値のコンマ区切りの組み合わせ。 `QuarantineState`</span><span class="sxs-lookup"><span data-stu-id="c5259-111">Comma-separated combination of the following values: `Full`, `QuarantineState`, `Watermark`, `Escrows`, `ConnectorDataStore`.</span></span> <span data-ttu-id="c5259-112">すべて`Full`のオプションを使用する場合に使用します。</span><span class="sxs-lookup"><span data-stu-id="c5259-112">Use `Full` if you want all of the options.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c5259-113">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c5259-113">JSON representation</span></span>

<span data-ttu-id="c5259-114">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c5259-114">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.synchronizationJobRestartCriteria"
}-->

```json
{
  "resetScope": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationJobRestartCriteria resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
