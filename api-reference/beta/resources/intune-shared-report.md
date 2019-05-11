---
title: レポート リソースの種類
description: 複数のワークフローをサポートする Microsoft Graph API for Intune のレポートリソースについて説明します。
localization_priority: Normal
author: rolyon
ms.prod: intune
ms.openlocfilehash: f94be1bcc5dfde092c6360bbdddd96d604d30a55
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33939673"
---
# <a name="report-resource-type"></a><span data-ttu-id="09749-103">レポート リソースの種類</span><span class="sxs-lookup"><span data-stu-id="09749-103">report resource type</span></span>

> <span data-ttu-id="09749-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="09749-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="09749-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="09749-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="09749-106">コンテキストに適した次の内容を返します。</span><span class="sxs-lookup"><span data-stu-id="09749-106">Returns the content appropriate for the context, including:</span></span>

- <span data-ttu-id="09749-107">デバイス構成プロファイルの履歴レポート。</span><span class="sxs-lookup"><span data-stu-id="09749-107">Device Configuration profile history reports.</span></span>
- <span data-ttu-id="09749-108">登録エラーレポート。</span><span class="sxs-lookup"><span data-stu-id="09749-108">Enrollment failure reports.</span></span>

## <a name="properties"></a><span data-ttu-id="09749-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="09749-109">Properties</span></span>
|<span data-ttu-id="09749-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="09749-110">Property</span></span>|<span data-ttu-id="09749-111">型</span><span class="sxs-lookup"><span data-stu-id="09749-111">Type</span></span>|<span data-ttu-id="09749-112">説明</span><span class="sxs-lookup"><span data-stu-id="09749-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="09749-113">content</span><span class="sxs-lookup"><span data-stu-id="09749-113">content</span></span>|<span data-ttu-id="09749-114">Stream</span><span class="sxs-lookup"><span data-stu-id="09749-114">Stream</span></span>|<span data-ttu-id="09749-115">レポートコンテンツ。詳細はレポートの種類によって異なります。</span><span class="sxs-lookup"><span data-stu-id="09749-115">Report content; details vary by report type.</span></span>|

## <a name="relationships"></a><span data-ttu-id="09749-116">関係</span><span class="sxs-lookup"><span data-stu-id="09749-116">Relationships</span></span>
<span data-ttu-id="09749-117">なし</span><span class="sxs-lookup"><span data-stu-id="09749-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="09749-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="09749-118">JSON Representation</span></span>
<span data-ttu-id="09749-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="09749-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.report"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.report",
  "content": "<Unknown Primitive Type Edm.Stream>"
}
```



