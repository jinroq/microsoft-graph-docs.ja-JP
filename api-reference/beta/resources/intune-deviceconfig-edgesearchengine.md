---
title: edgeSearchEngine リソースの種類
description: IT 管理者が MDM 制御デバイス用向けに事前定義されている既定の検索エンジンを設定できるようにします。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: b59fa163fe453d4f26dd71afa24edf9ac37d9d41
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27953239"
---
# <a name="edgesearchengine-resource-type"></a><span data-ttu-id="a2677-103">edgeSearchEngine リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a2677-103">edgeSearchEngine resource type</span></span>

> <span data-ttu-id="a2677-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="a2677-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a2677-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a2677-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a2677-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="a2677-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a2677-107">IT 管理者が MDM 制御デバイス用向けに事前定義されている既定の検索エンジンを設定できるようにします。</span><span class="sxs-lookup"><span data-stu-id="a2677-107">Allows IT admins to set a predefined default search engine for MDM-Controlled devices.</span></span>

<span data-ttu-id="a2677-108">[edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="a2677-108">Inherits from [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="a2677-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a2677-109">Properties</span></span>
|<span data-ttu-id="a2677-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a2677-110">Property</span></span>|<span data-ttu-id="a2677-111">種類</span><span class="sxs-lookup"><span data-stu-id="a2677-111">Type</span></span>|<span data-ttu-id="a2677-112">説明</span><span class="sxs-lookup"><span data-stu-id="a2677-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a2677-113">edgeSearchEngineType</span><span class="sxs-lookup"><span data-stu-id="a2677-113">edgeSearchEngineType</span></span>|[<span data-ttu-id="a2677-114">edgeSearchEngineType</span><span class="sxs-lookup"><span data-stu-id="a2677-114">edgeSearchEngineType</span></span>](../resources/intune-deviceconfig-edgesearchenginetype.md)|<span data-ttu-id="a2677-115">IT 管理者が MDM 制御デバイス用向けに事前定義されている既定の検索エンジンを設定できるようにします。</span><span class="sxs-lookup"><span data-stu-id="a2677-115">Allows IT admins to set a predefined default search engine for MDM-Controlled devices.</span></span> <span data-ttu-id="a2677-116">可能な値: `default`、`bing`。</span><span class="sxs-lookup"><span data-stu-id="a2677-116">Possible values are: `default`, `bing`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a2677-117">関係</span><span class="sxs-lookup"><span data-stu-id="a2677-117">Relationships</span></span>
<span data-ttu-id="a2677-118">なし</span><span class="sxs-lookup"><span data-stu-id="a2677-118">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="a2677-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a2677-119">JSON Representation</span></span>
<span data-ttu-id="a2677-120">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="a2677-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.edgeSearchEngine"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.edgeSearchEngine",
  "edgeSearchEngineType": "String"
}
```





