---
title: mobileContainedApp リソースの種類
description: パッケージとして機能する、mobileApp に含まれているアプリケーションを表す抽象クラスです。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: b81ee4ca194d1d01e3d834b3287f6b400e712a27
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27826286"
---
# <a name="mobilecontainedapp-resource-type"></a><span data-ttu-id="ee996-103">mobileContainedApp リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ee996-103">mobileContainedApp resource type</span></span>

> <span data-ttu-id="ee996-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="ee996-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ee996-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ee996-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ee996-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="ee996-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ee996-107">パッケージとして機能する、mobileApp に含まれているアプリケーションを表す抽象クラスです。</span><span class="sxs-lookup"><span data-stu-id="ee996-107">An abstract class that represents a contained app in a mobileApp acting as a package.</span></span>
## <a name="methods"></a><span data-ttu-id="ee996-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="ee996-108">Methods</span></span>
|<span data-ttu-id="ee996-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="ee996-109">Method</span></span>|<span data-ttu-id="ee996-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="ee996-110">Return Type</span></span>|<span data-ttu-id="ee996-111">説明</span><span class="sxs-lookup"><span data-stu-id="ee996-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ee996-112">リスト mobileContainedApps</span><span class="sxs-lookup"><span data-stu-id="ee996-112">List mobileContainedApps</span></span>](../api/intune-apps-mobilecontainedapp-list.md)|<span data-ttu-id="ee996-113">[mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="ee996-113">[mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) collection</span></span>|<span data-ttu-id="ee996-114">[MobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)オブジェクトのプロパティと関係を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="ee996-114">List properties and relationships of the [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) objects.</span></span>|
|[<span data-ttu-id="ee996-115">MobileContainedApp を取得します。</span><span class="sxs-lookup"><span data-stu-id="ee996-115">Get mobileContainedApp</span></span>](../api/intune-apps-mobilecontainedapp-get.md)|[<span data-ttu-id="ee996-116">mobileContainedApp</span><span class="sxs-lookup"><span data-stu-id="ee996-116">mobileContainedApp</span></span>](../resources/intune-apps-mobilecontainedapp.md)|<span data-ttu-id="ee996-117">[MobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ee996-117">Read properties and relationships of the [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="ee996-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ee996-118">Properties</span></span>
|<span data-ttu-id="ee996-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ee996-119">Property</span></span>|<span data-ttu-id="ee996-120">種類</span><span class="sxs-lookup"><span data-stu-id="ee996-120">Type</span></span>|<span data-ttu-id="ee996-121">説明</span><span class="sxs-lookup"><span data-stu-id="ee996-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ee996-122">ID</span><span class="sxs-lookup"><span data-stu-id="ee996-122">id</span></span>|<span data-ttu-id="ee996-123">String</span><span class="sxs-lookup"><span data-stu-id="ee996-123">String</span></span>|<span data-ttu-id="ee996-124">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="ee996-124">Key of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ee996-125">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ee996-125">Relationships</span></span>
<span data-ttu-id="ee996-126">なし</span><span class="sxs-lookup"><span data-stu-id="ee996-126">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="ee996-127">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ee996-127">JSON Representation</span></span>
<span data-ttu-id="ee996-128">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="ee996-128">Here is a JSON representation of the resource.</span></span>
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





