---
title: edgeSearchEngine リソースの種類
description: IT 管理者が MDM 制御デバイス用向けに事前定義されている既定の検索エンジンを設定できるようにします。
ms.openlocfilehash: 4da5008eda31bb393ed25048c5d94724d2174e3f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27021929"
---
# <a name="edgesearchengine-resource-type"></a><span data-ttu-id="81025-103">edgeSearchEngine リソースの種類</span><span class="sxs-lookup"><span data-stu-id="81025-103">edgeSearchEngine resource type</span></span>

> <span data-ttu-id="81025-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="81025-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="81025-105">IT 管理者が MDM 制御デバイス用向けに事前定義されている既定の検索エンジンを設定できるようにします。</span><span class="sxs-lookup"><span data-stu-id="81025-105">Allows IT admins to set a predefined default search engine for MDM-Controlled devices.</span></span>

<span data-ttu-id="81025-106">[edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="81025-106">Inherits from [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="81025-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="81025-107">Properties</span></span>
|<span data-ttu-id="81025-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="81025-108">Property</span></span>|<span data-ttu-id="81025-109">型</span><span class="sxs-lookup"><span data-stu-id="81025-109">Type</span></span>|<span data-ttu-id="81025-110">説明</span><span class="sxs-lookup"><span data-stu-id="81025-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="81025-111">edgeSearchEngineType</span><span class="sxs-lookup"><span data-stu-id="81025-111">edgeSearchEngineType</span></span>|[<span data-ttu-id="81025-112">edgeSearchEngineType</span><span class="sxs-lookup"><span data-stu-id="81025-112">edgeSearchEngineType</span></span>](../resources/intune-deviceconfig-edgesearchenginetype.md)|<span data-ttu-id="81025-113">IT 管理者が MDM 制御デバイス用向けに事前定義されている既定の検索エンジンを設定できるようにします。</span><span class="sxs-lookup"><span data-stu-id="81025-113">Allows IT admins to set a predefined default search engine for MDM-Controlled devices.</span></span> <span data-ttu-id="81025-114">可能な値: `default`、`bing`。</span><span class="sxs-lookup"><span data-stu-id="81025-114">Possible values are: `default`, `bing`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="81025-115">関係</span><span class="sxs-lookup"><span data-stu-id="81025-115">Relationships</span></span>
<span data-ttu-id="81025-116">なし</span><span class="sxs-lookup"><span data-stu-id="81025-116">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="81025-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="81025-117">JSON Representation</span></span>
<span data-ttu-id="81025-118">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="81025-118">Here is a JSON representation of the resource.</span></span>
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



