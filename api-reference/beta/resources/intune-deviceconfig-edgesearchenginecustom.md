---
title: edgeSearchEngineCustom リソースの種類
description: IT 管理者が MDM 制御デバイス用向けのカスタムの既定の検索エンジンを設定できるようにします。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 34e31bb35426f7aab1b2a8e824e50933e5892b5e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36001419"
---
# <a name="edgesearchenginecustom-resource-type"></a><span data-ttu-id="e06c5-103">edgeSearchEngineCustom リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e06c5-103">edgeSearchEngineCustom resource type</span></span>

> <span data-ttu-id="e06c5-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e06c5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e06c5-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="e06c5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e06c5-106">IT 管理者が MDM 制御デバイス用向けのカスタムの既定の検索エンジンを設定できるようにします。</span><span class="sxs-lookup"><span data-stu-id="e06c5-106">Allows IT admins to set a custom default search engine for MDM-Controlled devices.</span></span>


<span data-ttu-id="e06c5-107">[edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="e06c5-107">Inherits from [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="e06c5-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e06c5-108">Properties</span></span>
|<span data-ttu-id="e06c5-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e06c5-109">Property</span></span>|<span data-ttu-id="e06c5-110">型</span><span class="sxs-lookup"><span data-stu-id="e06c5-110">Type</span></span>|<span data-ttu-id="e06c5-111">説明</span><span class="sxs-lookup"><span data-stu-id="e06c5-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e06c5-112">edgeSearchEngineOpenSearchXmlUrl</span><span class="sxs-lookup"><span data-stu-id="e06c5-112">edgeSearchEngineOpenSearchXmlUrl</span></span>|<span data-ttu-id="e06c5-113">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="e06c5-113">String</span></span>|<span data-ttu-id="e06c5-114">短縮名と検索エンジンの URL が最低限含まれる OpenSearch xml ファイルが入っている https リンクを指します。</span><span class="sxs-lookup"><span data-stu-id="e06c5-114">Points to a https link containing the OpenSearch xml file that contains, at minimum, the short name and the URL to the search Engine.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e06c5-115">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e06c5-115">Relationships</span></span>
<span data-ttu-id="e06c5-116">なし</span><span class="sxs-lookup"><span data-stu-id="e06c5-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e06c5-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e06c5-117">JSON Representation</span></span>
<span data-ttu-id="e06c5-118">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="e06c5-118">Here is a JSON representation of the resource.</span></span>
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





