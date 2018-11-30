---
title: edgeSearchEngine リソースの種類
description: IT 管理者が MDM 制御デバイス用向けに事前定義されている既定の検索エンジンを設定できるようにします。
ms.openlocfilehash: 51f947911e73927816eb4f1150cab36cba904f58
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27066500"
---
# <a name="edgesearchengine-resource-type"></a><span data-ttu-id="76b48-103">edgeSearchEngine リソースの種類</span><span class="sxs-lookup"><span data-stu-id="76b48-103">edgeSearchEngine resource type</span></span>

> <span data-ttu-id="76b48-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="76b48-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="76b48-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="76b48-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="76b48-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="76b48-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="76b48-107">IT 管理者が MDM 制御デバイス用向けに事前定義されている既定の検索エンジンを設定できるようにします。</span><span class="sxs-lookup"><span data-stu-id="76b48-107">Allows IT admins to set a predefined default search engine for MDM-Controlled devices.</span></span>

<span data-ttu-id="76b48-108">[edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="76b48-108">Inherits from [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="76b48-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="76b48-109">Properties</span></span>
|<span data-ttu-id="76b48-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="76b48-110">Property</span></span>|<span data-ttu-id="76b48-111">型</span><span class="sxs-lookup"><span data-stu-id="76b48-111">Type</span></span>|<span data-ttu-id="76b48-112">説明</span><span class="sxs-lookup"><span data-stu-id="76b48-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="76b48-113">edgeSearchEngineType</span><span class="sxs-lookup"><span data-stu-id="76b48-113">edgeSearchEngineType</span></span>|[<span data-ttu-id="76b48-114">edgeSearchEngineType</span><span class="sxs-lookup"><span data-stu-id="76b48-114">edgeSearchEngineType</span></span>](../resources/intune-deviceconfig-edgesearchenginetype.md)|<span data-ttu-id="76b48-115">IT 管理者が MDM 制御デバイス用向けに事前定義されている既定の検索エンジンを設定できるようにします。</span><span class="sxs-lookup"><span data-stu-id="76b48-115">Allows IT admins to set a predefined default search engine for MDM-Controlled devices.</span></span> <span data-ttu-id="76b48-116">可能な値: `default`、`bing`。</span><span class="sxs-lookup"><span data-stu-id="76b48-116">Possible values are: `default`, `bing`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="76b48-117">関係</span><span class="sxs-lookup"><span data-stu-id="76b48-117">Relationships</span></span>
<span data-ttu-id="76b48-118">なし</span><span class="sxs-lookup"><span data-stu-id="76b48-118">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="76b48-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="76b48-119">JSON Representation</span></span>
<span data-ttu-id="76b48-120">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="76b48-120">Here is a JSON representation of the resource.</span></span>
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





