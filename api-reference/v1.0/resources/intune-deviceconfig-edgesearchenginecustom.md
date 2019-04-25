---
title: edgeSearchEngineCustom リソースの種類
description: IT 管理者が MDM 制御デバイス用向けのカスタムの既定の検索エンジンを設定できるようにします。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 523a2de33619886997cbcb052079bbf2937c9d48
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32541228"
---
# <a name="edgesearchenginecustom-resource-type"></a><span data-ttu-id="dfe03-103">edgeSearchEngineCustom リソースの種類</span><span class="sxs-lookup"><span data-stu-id="dfe03-103">edgeSearchEngineCustom resource type</span></span>

> <span data-ttu-id="dfe03-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="dfe03-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dfe03-105">IT 管理者が MDM 制御デバイス用向けのカスタムの既定の検索エンジンを設定できるようにします。</span><span class="sxs-lookup"><span data-stu-id="dfe03-105">Allows IT admins to set a custom default search engine for MDM-Controlled devices.</span></span>


<span data-ttu-id="dfe03-106">[edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="dfe03-106">Inherits from [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="dfe03-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="dfe03-107">Properties</span></span>
|<span data-ttu-id="dfe03-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="dfe03-108">Property</span></span>|<span data-ttu-id="dfe03-109">型</span><span class="sxs-lookup"><span data-stu-id="dfe03-109">Type</span></span>|<span data-ttu-id="dfe03-110">説明</span><span class="sxs-lookup"><span data-stu-id="dfe03-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dfe03-111">edgeSearchEngineOpenSearchXmlUrl</span><span class="sxs-lookup"><span data-stu-id="dfe03-111">edgeSearchEngineOpenSearchXmlUrl</span></span>|<span data-ttu-id="dfe03-112">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="dfe03-112">String</span></span>|<span data-ttu-id="dfe03-113">短縮名と検索エンジンの URL が最低限含まれる OpenSearch xml ファイルが入っている https リンクを指します。</span><span class="sxs-lookup"><span data-stu-id="dfe03-113">Points to a https link containing the OpenSearch xml file that contains, at minimum, the short name and the URL to the search Engine.</span></span>|

## <a name="relationships"></a><span data-ttu-id="dfe03-114">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="dfe03-114">Relationships</span></span>
<span data-ttu-id="dfe03-115">なし</span><span class="sxs-lookup"><span data-stu-id="dfe03-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="dfe03-116">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="dfe03-116">JSON Representation</span></span>
<span data-ttu-id="dfe03-117">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="dfe03-117">Here is a JSON representation of the resource.</span></span>
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



