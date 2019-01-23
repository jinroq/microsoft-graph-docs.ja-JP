---
title: mobileContainedApp リソースの種類
description: パッケージとして機能する、mobileApp に含まれているアプリケーションを表す抽象クラスです。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c5d4ed392d681d97478cb1baf5ff6f854cb74011
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425667"
---
# <a name="mobilecontainedapp-resource-type"></a><span data-ttu-id="c6b21-103">mobileContainedApp リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c6b21-103">mobileContainedApp resource type</span></span>

> <span data-ttu-id="c6b21-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c6b21-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c6b21-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c6b21-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c6b21-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="c6b21-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c6b21-107">パッケージとして機能する、mobileApp に含まれているアプリケーションを表す抽象クラスです。</span><span class="sxs-lookup"><span data-stu-id="c6b21-107">An abstract class that represents a contained app in a mobileApp acting as a package.</span></span>

## <a name="methods"></a><span data-ttu-id="c6b21-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="c6b21-108">Methods</span></span>
|<span data-ttu-id="c6b21-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="c6b21-109">Method</span></span>|<span data-ttu-id="c6b21-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="c6b21-110">Return Type</span></span>|<span data-ttu-id="c6b21-111">説明</span><span class="sxs-lookup"><span data-stu-id="c6b21-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c6b21-112">リスト mobileContainedApps</span><span class="sxs-lookup"><span data-stu-id="c6b21-112">List mobileContainedApps</span></span>](../api/intune-apps-mobilecontainedapp-list.md)|<span data-ttu-id="c6b21-113">[mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="c6b21-113">[mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) collection</span></span>|<span data-ttu-id="c6b21-114">[MobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)オブジェクトのプロパティと関係を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="c6b21-114">List properties and relationships of the [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) objects.</span></span>|
|[<span data-ttu-id="c6b21-115">MobileContainedApp を取得します。</span><span class="sxs-lookup"><span data-stu-id="c6b21-115">Get mobileContainedApp</span></span>](../api/intune-apps-mobilecontainedapp-get.md)|[<span data-ttu-id="c6b21-116">mobileContainedApp</span><span class="sxs-lookup"><span data-stu-id="c6b21-116">mobileContainedApp</span></span>](../resources/intune-apps-mobilecontainedapp.md)|<span data-ttu-id="c6b21-117">[MobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c6b21-117">Read properties and relationships of the [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="c6b21-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c6b21-118">Properties</span></span>
|<span data-ttu-id="c6b21-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c6b21-119">Property</span></span>|<span data-ttu-id="c6b21-120">型</span><span class="sxs-lookup"><span data-stu-id="c6b21-120">Type</span></span>|<span data-ttu-id="c6b21-121">説明</span><span class="sxs-lookup"><span data-stu-id="c6b21-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c6b21-122">id</span><span class="sxs-lookup"><span data-stu-id="c6b21-122">id</span></span>|<span data-ttu-id="c6b21-123">String</span><span class="sxs-lookup"><span data-stu-id="c6b21-123">String</span></span>|<span data-ttu-id="c6b21-124">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="c6b21-124">Key of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c6b21-125">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="c6b21-125">Relationships</span></span>
<span data-ttu-id="c6b21-126">なし</span><span class="sxs-lookup"><span data-stu-id="c6b21-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c6b21-127">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c6b21-127">JSON Representation</span></span>
<span data-ttu-id="c6b21-128">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="c6b21-128">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileContainedApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileContainedApp",
  "id": "String (identifier)"
}
```




