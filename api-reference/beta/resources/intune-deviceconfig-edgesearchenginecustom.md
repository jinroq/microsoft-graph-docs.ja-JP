---
title: edgeSearchEngineCustom リソースの種類
description: IT 管理者が MDM 制御デバイス用向けのカスタムの既定の検索エンジンを設定できるようにします。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: de856edf13a8d97e54925ca42537e977351675d7
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33946708"
---
# <a name="edgesearchenginecustom-resource-type"></a><span data-ttu-id="b9a96-103">edgeSearchEngineCustom リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b9a96-103">edgeSearchEngineCustom resource type</span></span>

> <span data-ttu-id="b9a96-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b9a96-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b9a96-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="b9a96-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b9a96-106">IT 管理者が MDM 制御デバイス用向けのカスタムの既定の検索エンジンを設定できるようにします。</span><span class="sxs-lookup"><span data-stu-id="b9a96-106">Allows IT admins to set a custom default search engine for MDM-Controlled devices.</span></span>


<span data-ttu-id="b9a96-107">[edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="b9a96-107">Inherits from [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="b9a96-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b9a96-108">Properties</span></span>
|<span data-ttu-id="b9a96-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b9a96-109">Property</span></span>|<span data-ttu-id="b9a96-110">型</span><span class="sxs-lookup"><span data-stu-id="b9a96-110">Type</span></span>|<span data-ttu-id="b9a96-111">説明</span><span class="sxs-lookup"><span data-stu-id="b9a96-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b9a96-112">edgeSearchEngineOpenSearchXmlUrl</span><span class="sxs-lookup"><span data-stu-id="b9a96-112">edgeSearchEngineOpenSearchXmlUrl</span></span>|<span data-ttu-id="b9a96-113">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="b9a96-113">String</span></span>|<span data-ttu-id="b9a96-114">短縮名と検索エンジンの URL が最低限含まれる OpenSearch xml ファイルが入っている https リンクを指します。</span><span class="sxs-lookup"><span data-stu-id="b9a96-114">Points to a https link containing the OpenSearch xml file that contains, at minimum, the short name and the URL to the search Engine.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b9a96-115">関係</span><span class="sxs-lookup"><span data-stu-id="b9a96-115">Relationships</span></span>
<span data-ttu-id="b9a96-116">なし</span><span class="sxs-lookup"><span data-stu-id="b9a96-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b9a96-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b9a96-117">JSON Representation</span></span>
<span data-ttu-id="b9a96-118">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="b9a96-118">Here is a JSON representation of the resource.</span></span>
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




