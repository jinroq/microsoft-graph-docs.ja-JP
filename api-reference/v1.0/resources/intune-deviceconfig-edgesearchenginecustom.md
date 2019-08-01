---
title: edgeSearchEngineCustom リソースの種類
description: IT 管理者が MDM 制御デバイス用向けのカスタムの既定の検索エンジンを設定できるようにします。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 367c81764bbf54cef8e5645c08fcb93ec430518d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36028330"
---
# <a name="edgesearchenginecustom-resource-type"></a><span data-ttu-id="60b7c-103">edgeSearchEngineCustom リソースの種類</span><span class="sxs-lookup"><span data-stu-id="60b7c-103">edgeSearchEngineCustom resource type</span></span>

> <span data-ttu-id="60b7c-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="60b7c-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="60b7c-105">IT 管理者が MDM 制御デバイス用向けのカスタムの既定の検索エンジンを設定できるようにします。</span><span class="sxs-lookup"><span data-stu-id="60b7c-105">Allows IT admins to set a custom default search engine for MDM-Controlled devices.</span></span>


<span data-ttu-id="60b7c-106">[edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="60b7c-106">Inherits from [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="60b7c-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="60b7c-107">Properties</span></span>
|<span data-ttu-id="60b7c-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="60b7c-108">Property</span></span>|<span data-ttu-id="60b7c-109">型</span><span class="sxs-lookup"><span data-stu-id="60b7c-109">Type</span></span>|<span data-ttu-id="60b7c-110">説明</span><span class="sxs-lookup"><span data-stu-id="60b7c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="60b7c-111">edgeSearchEngineOpenSearchXmlUrl</span><span class="sxs-lookup"><span data-stu-id="60b7c-111">edgeSearchEngineOpenSearchXmlUrl</span></span>|<span data-ttu-id="60b7c-112">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="60b7c-112">String</span></span>|<span data-ttu-id="60b7c-113">短縮名と検索エンジンの URL が最低限含まれる OpenSearch xml ファイルが入っている https リンクを指します。</span><span class="sxs-lookup"><span data-stu-id="60b7c-113">Points to a https link containing the OpenSearch xml file that contains, at minimum, the short name and the URL to the search Engine.</span></span>|

## <a name="relationships"></a><span data-ttu-id="60b7c-114">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="60b7c-114">Relationships</span></span>
<span data-ttu-id="60b7c-115">なし</span><span class="sxs-lookup"><span data-stu-id="60b7c-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="60b7c-116">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="60b7c-116">JSON Representation</span></span>
<span data-ttu-id="60b7c-117">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="60b7c-117">Here is a JSON representation of the resource.</span></span>
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



