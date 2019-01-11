---
title: synchronizationJobRestartCriteria リソースの種類
description: 'スコープを定義します[synchronizationJob: 再起動](../api/synchronization_synchronizationjob_restart.md)アクション。'
localization_priority: Normal
ms.openlocfilehash: e26bae2e418da22a2b56e3acb973e4111066df23
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27867880"
---
# <a name="synchronizationjobrestartcriteria-resource-type"></a><span data-ttu-id="f7ce8-103">synchronizationJobRestartCriteria リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f7ce8-103">synchronizationJobRestartCriteria resource type</span></span>

> <span data-ttu-id="f7ce8-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="f7ce8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f7ce8-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f7ce8-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f7ce8-106">スコープを定義します[synchronizationJob: 再起動](../api/synchronization_synchronizationjob_restart.md)アクション。</span><span class="sxs-lookup"><span data-stu-id="f7ce8-106">Defines the scope of the [synchronizationJob: restart](../api/synchronization_synchronizationjob_restart.md) action.</span></span>

## <a name="properties"></a><span data-ttu-id="f7ce8-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f7ce8-107">Properties</span></span>
| <span data-ttu-id="f7ce8-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f7ce8-108">Property</span></span>     | <span data-ttu-id="f7ce8-109">種類</span><span class="sxs-lookup"><span data-stu-id="f7ce8-109">Type</span></span>   |<span data-ttu-id="f7ce8-110">説明</span><span class="sxs-lookup"><span data-stu-id="f7ce8-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f7ce8-111">resetScope</span><span class="sxs-lookup"><span data-stu-id="f7ce8-111">resetScope</span></span>|<span data-ttu-id="f7ce8-112">String</span><span class="sxs-lookup"><span data-stu-id="f7ce8-112">String</span></span>| <span data-ttu-id="f7ce8-113">次の値のコンマ区切りの組み合わせ: `Full`、 `QuarantineState`、 `Watermark`、 `Escrows`、 `ConnectorDataStore`。</span><span class="sxs-lookup"><span data-stu-id="f7ce8-113">Comma-separated combination of the following values: `Full`, `QuarantineState`, `Watermark`, `Escrows`, `ConnectorDataStore`.</span></span> <span data-ttu-id="f7ce8-114">使用`Full`のすべてのオプションにする場合。</span><span class="sxs-lookup"><span data-stu-id="f7ce8-114">Use `Full` if you want all of the options.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f7ce8-115">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f7ce8-115">JSON representation</span></span>

<span data-ttu-id="f7ce8-116">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f7ce8-116">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "synchronizationJobRestartCriteria resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
