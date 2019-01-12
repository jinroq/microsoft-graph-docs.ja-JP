---
title: edgeSearchEngine リソースの種類
description: IT 管理者が MDM 制御デバイス用向けに事前定義されている既定の検索エンジンを設定できるようにします。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 87a072ca6fb325f599c51a219bfa0e9d2ad0ac0d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27935620"
---
# <a name="edgesearchengine-resource-type"></a><span data-ttu-id="0c0b7-103">edgeSearchEngine リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0c0b7-103">edgeSearchEngine resource type</span></span>

> <span data-ttu-id="0c0b7-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="0c0b7-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0c0b7-105">IT 管理者が MDM 制御デバイス用向けに事前定義されている既定の検索エンジンを設定できるようにします。</span><span class="sxs-lookup"><span data-stu-id="0c0b7-105">Allows IT admins to set a predefined default search engine for MDM-Controlled devices.</span></span>

<span data-ttu-id="0c0b7-106">[edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="0c0b7-106">Inherits from [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="0c0b7-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0c0b7-107">Properties</span></span>
|<span data-ttu-id="0c0b7-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0c0b7-108">Property</span></span>|<span data-ttu-id="0c0b7-109">種類</span><span class="sxs-lookup"><span data-stu-id="0c0b7-109">Type</span></span>|<span data-ttu-id="0c0b7-110">説明</span><span class="sxs-lookup"><span data-stu-id="0c0b7-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0c0b7-111">edgeSearchEngineType</span><span class="sxs-lookup"><span data-stu-id="0c0b7-111">edgeSearchEngineType</span></span>|[<span data-ttu-id="0c0b7-112">edgeSearchEngineType</span><span class="sxs-lookup"><span data-stu-id="0c0b7-112">edgeSearchEngineType</span></span>](../resources/intune-deviceconfig-edgesearchenginetype.md)|<span data-ttu-id="0c0b7-113">IT 管理者が MDM 制御デバイス用向けに事前定義されている既定の検索エンジンを設定できるようにします。</span><span class="sxs-lookup"><span data-stu-id="0c0b7-113">Allows IT admins to set a predefined default search engine for MDM-Controlled devices.</span></span> <span data-ttu-id="0c0b7-114">可能な値: `default`、`bing`。</span><span class="sxs-lookup"><span data-stu-id="0c0b7-114">Possible values are: `default`, `bing`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0c0b7-115">関係</span><span class="sxs-lookup"><span data-stu-id="0c0b7-115">Relationships</span></span>
<span data-ttu-id="0c0b7-116">なし</span><span class="sxs-lookup"><span data-stu-id="0c0b7-116">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="0c0b7-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0c0b7-117">JSON Representation</span></span>
<span data-ttu-id="0c0b7-118">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="0c0b7-118">Here is a JSON representation of the resource.</span></span>
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



