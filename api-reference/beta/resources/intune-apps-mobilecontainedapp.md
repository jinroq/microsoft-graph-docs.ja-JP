---
title: mobileContainedApp リソースの種類
description: パッケージとして機能する mobileApp に含まれているアプリを表す抽象クラス。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 500d8329f998f340468b676d054211392ae6a6a4
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33949907"
---
# <a name="mobilecontainedapp-resource-type"></a><span data-ttu-id="b44e6-103">mobileContainedApp リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b44e6-103">mobileContainedApp resource type</span></span>

> <span data-ttu-id="b44e6-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b44e6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b44e6-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="b44e6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b44e6-106">パッケージとして機能する mobileApp に含まれているアプリを表す抽象クラス。</span><span class="sxs-lookup"><span data-stu-id="b44e6-106">An abstract class that represents a contained app in a mobileApp acting as a package.</span></span>

## <a name="methods"></a><span data-ttu-id="b44e6-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="b44e6-107">Methods</span></span>
|<span data-ttu-id="b44e6-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="b44e6-108">Method</span></span>|<span data-ttu-id="b44e6-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="b44e6-109">Return Type</span></span>|<span data-ttu-id="b44e6-110">説明</span><span class="sxs-lookup"><span data-stu-id="b44e6-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="b44e6-111">リスト mobileContainedApps</span><span class="sxs-lookup"><span data-stu-id="b44e6-111">List mobileContainedApps</span></span>](../api/intune-apps-mobilecontainedapp-list.md)|<span data-ttu-id="b44e6-112">[mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="b44e6-112">[mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) collection</span></span>|<span data-ttu-id="b44e6-113">[MobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="b44e6-113">List properties and relationships of the [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) objects.</span></span>|
|[<span data-ttu-id="b44e6-114">MobileContainedApp を取得する</span><span class="sxs-lookup"><span data-stu-id="b44e6-114">Get mobileContainedApp</span></span>](../api/intune-apps-mobilecontainedapp-get.md)|[<span data-ttu-id="b44e6-115">mobileContainedApp</span><span class="sxs-lookup"><span data-stu-id="b44e6-115">mobileContainedApp</span></span>](../resources/intune-apps-mobilecontainedapp.md)|<span data-ttu-id="b44e6-116">[MobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="b44e6-116">Read properties and relationships of the [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="b44e6-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b44e6-117">Properties</span></span>
|<span data-ttu-id="b44e6-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b44e6-118">Property</span></span>|<span data-ttu-id="b44e6-119">型</span><span class="sxs-lookup"><span data-stu-id="b44e6-119">Type</span></span>|<span data-ttu-id="b44e6-120">説明</span><span class="sxs-lookup"><span data-stu-id="b44e6-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b44e6-121">id</span><span class="sxs-lookup"><span data-stu-id="b44e6-121">id</span></span>|<span data-ttu-id="b44e6-122">String</span><span class="sxs-lookup"><span data-stu-id="b44e6-122">String</span></span>|<span data-ttu-id="b44e6-123">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="b44e6-123">Key of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b44e6-124">関係</span><span class="sxs-lookup"><span data-stu-id="b44e6-124">Relationships</span></span>
<span data-ttu-id="b44e6-125">なし</span><span class="sxs-lookup"><span data-stu-id="b44e6-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b44e6-126">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b44e6-126">JSON Representation</span></span>
<span data-ttu-id="b44e6-127">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="b44e6-127">Here is a JSON representation of the resource.</span></span>
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




