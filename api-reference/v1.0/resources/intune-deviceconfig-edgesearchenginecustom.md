---
title: edgeSearchEngineCustom リソースの種類
description: IT 管理者が MDM 制御デバイス用向けのカスタムの既定の検索エンジンを設定できるようにします。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 38308433f5e68d921a98e7b030540c465b33fe44
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27957936"
---
# <a name="edgesearchenginecustom-resource-type"></a><span data-ttu-id="bff5c-103">edgeSearchEngineCustom リソースの種類</span><span class="sxs-lookup"><span data-stu-id="bff5c-103">edgeSearchEngineCustom resource type</span></span>

> <span data-ttu-id="bff5c-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="bff5c-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bff5c-105">IT 管理者が MDM 制御デバイス用向けのカスタムの既定の検索エンジンを設定できるようにします。</span><span class="sxs-lookup"><span data-stu-id="bff5c-105">Allows IT admins to set a custom default search engine for MDM-Controlled devices.</span></span>

<span data-ttu-id="bff5c-106">[edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="bff5c-106">Inherits from [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="bff5c-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bff5c-107">Properties</span></span>
|<span data-ttu-id="bff5c-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bff5c-108">Property</span></span>|<span data-ttu-id="bff5c-109">種類</span><span class="sxs-lookup"><span data-stu-id="bff5c-109">Type</span></span>|<span data-ttu-id="bff5c-110">説明</span><span class="sxs-lookup"><span data-stu-id="bff5c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bff5c-111">edgeSearchEngineOpenSearchXmlUrl</span><span class="sxs-lookup"><span data-stu-id="bff5c-111">edgeSearchEngineOpenSearchXmlUrl</span></span>|<span data-ttu-id="bff5c-112">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="bff5c-112">String</span></span>|<span data-ttu-id="bff5c-113">短縮名と検索エンジンの URL が最低限含まれる OpenSearch xml ファイルが入っている https リンクを指します。</span><span class="sxs-lookup"><span data-stu-id="bff5c-113">Points to a https link containing the OpenSearch xml file that contains, at minimum, the short name and the URL to the search Engine.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bff5c-114">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="bff5c-114">Relationships</span></span>
<span data-ttu-id="bff5c-115">なし</span><span class="sxs-lookup"><span data-stu-id="bff5c-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="bff5c-116">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="bff5c-116">JSON Representation</span></span>
<span data-ttu-id="bff5c-117">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="bff5c-117">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.edgeSearchEngineCustom"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.edgeSearchEngineCustom",
  "edgeSearchEngineOpenSearchXmlUrl": "String"
}
```



