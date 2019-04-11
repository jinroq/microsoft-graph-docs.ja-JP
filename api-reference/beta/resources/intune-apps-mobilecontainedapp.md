---
title: mobileContainedApp リソースの種類
description: パッケージとして機能する mobileApp に含まれているアプリを表す抽象クラス。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 05874102e62e86e5b64fb20c892c2e96c66acfc9
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31795136"
---
# <a name="mobilecontainedapp-resource-type"></a><span data-ttu-id="50794-103">mobileContainedApp リソースの種類</span><span class="sxs-lookup"><span data-stu-id="50794-103">mobileContainedApp resource type</span></span>

> <span data-ttu-id="50794-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="50794-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="50794-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="50794-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="50794-106">パッケージとして機能する mobileApp に含まれているアプリを表す抽象クラス。</span><span class="sxs-lookup"><span data-stu-id="50794-106">An abstract class that represents a contained app in a mobileApp acting as a package.</span></span>

## <a name="methods"></a><span data-ttu-id="50794-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="50794-107">Methods</span></span>
|<span data-ttu-id="50794-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="50794-108">Method</span></span>|<span data-ttu-id="50794-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="50794-109">Return Type</span></span>|<span data-ttu-id="50794-110">説明</span><span class="sxs-lookup"><span data-stu-id="50794-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="50794-111">リスト mobileContainedApps</span><span class="sxs-lookup"><span data-stu-id="50794-111">List mobileContainedApps</span></span>](../api/intune-apps-mobilecontainedapp-list.md)|<span data-ttu-id="50794-112">[mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="50794-112">[mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) collection</span></span>|<span data-ttu-id="50794-113">[mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="50794-113">List properties and relationships of the [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) objects.</span></span>|
|[<span data-ttu-id="50794-114">mobileContainedApp を取得する</span><span class="sxs-lookup"><span data-stu-id="50794-114">Get mobileContainedApp</span></span>](../api/intune-apps-mobilecontainedapp-get.md)|[<span data-ttu-id="50794-115">mobileContainedApp</span><span class="sxs-lookup"><span data-stu-id="50794-115">mobileContainedApp</span></span>](../resources/intune-apps-mobilecontainedapp.md)|<span data-ttu-id="50794-116">[mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="50794-116">Read properties and relationships of the [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="50794-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="50794-117">Properties</span></span>
|<span data-ttu-id="50794-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="50794-118">Property</span></span>|<span data-ttu-id="50794-119">型</span><span class="sxs-lookup"><span data-stu-id="50794-119">Type</span></span>|<span data-ttu-id="50794-120">説明</span><span class="sxs-lookup"><span data-stu-id="50794-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="50794-121">id</span><span class="sxs-lookup"><span data-stu-id="50794-121">id</span></span>|<span data-ttu-id="50794-122">String</span><span class="sxs-lookup"><span data-stu-id="50794-122">String</span></span>|<span data-ttu-id="50794-123">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="50794-123">Key of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="50794-124">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="50794-124">Relationships</span></span>
<span data-ttu-id="50794-125">なし</span><span class="sxs-lookup"><span data-stu-id="50794-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="50794-126">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="50794-126">JSON Representation</span></span>
<span data-ttu-id="50794-127">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="50794-127">Here is a JSON representation of the resource.</span></span>
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





