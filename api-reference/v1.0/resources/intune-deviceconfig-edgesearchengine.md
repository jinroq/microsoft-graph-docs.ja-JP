---
title: edgeSearchEngine リソースの種類
description: IT 管理者が MDM 制御デバイス用向けに事前定義されている既定の検索エンジンを設定できるようにします。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 7a58cbed251773559beb2589893ab9759d4758fa
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27819909"
---
# <a name="edgesearchengine-resource-type"></a><span data-ttu-id="5b528-103">edgeSearchEngine リソースの種類</span><span class="sxs-lookup"><span data-stu-id="5b528-103">edgeSearchEngine resource type</span></span>

> <span data-ttu-id="5b528-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="5b528-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5b528-105">IT 管理者が MDM 制御デバイス用向けに事前定義されている既定の検索エンジンを設定できるようにします。</span><span class="sxs-lookup"><span data-stu-id="5b528-105">Allows IT admins to set a predefined default search engine for MDM-Controlled devices.</span></span>

<span data-ttu-id="5b528-106">[edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="5b528-106">Inherits from [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="5b528-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5b528-107">Properties</span></span>
|<span data-ttu-id="5b528-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5b528-108">Property</span></span>|<span data-ttu-id="5b528-109">種類</span><span class="sxs-lookup"><span data-stu-id="5b528-109">Type</span></span>|<span data-ttu-id="5b528-110">説明</span><span class="sxs-lookup"><span data-stu-id="5b528-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5b528-111">edgeSearchEngineType</span><span class="sxs-lookup"><span data-stu-id="5b528-111">edgeSearchEngineType</span></span>|[<span data-ttu-id="5b528-112">edgeSearchEngineType</span><span class="sxs-lookup"><span data-stu-id="5b528-112">edgeSearchEngineType</span></span>](../resources/intune-deviceconfig-edgesearchenginetype.md)|<span data-ttu-id="5b528-113">IT 管理者が MDM 制御デバイス用向けに事前定義されている既定の検索エンジンを設定できるようにします。</span><span class="sxs-lookup"><span data-stu-id="5b528-113">Allows IT admins to set a predefined default search engine for MDM-Controlled devices.</span></span> <span data-ttu-id="5b528-114">可能な値: `default`、`bing`。</span><span class="sxs-lookup"><span data-stu-id="5b528-114">Possible values are: `default`, `bing`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5b528-115">関係</span><span class="sxs-lookup"><span data-stu-id="5b528-115">Relationships</span></span>
<span data-ttu-id="5b528-116">なし</span><span class="sxs-lookup"><span data-stu-id="5b528-116">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="5b528-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="5b528-117">JSON Representation</span></span>
<span data-ttu-id="5b528-118">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="5b528-118">Here is a JSON representation of the resource.</span></span>
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



