---
title: iosHomeScreenFolderPage リソースの種類
description: ホーム画面上のアプリが含まれるフォルダー
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2808adaa99787efb96c7b21deaddf4c855e799d6
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30165528"
---
# <a name="ioshomescreenfolderpage-resource-type"></a><span data-ttu-id="d1925-103">iosHomeScreenFolderPage リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d1925-103">iosHomeScreenFolderPage resource type</span></span>

> <span data-ttu-id="d1925-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d1925-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d1925-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="d1925-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d1925-106">ホーム画面上のアプリが含まれるフォルダー</span><span class="sxs-lookup"><span data-stu-id="d1925-106">A folder containing apps on the Home Screen</span></span>

## <a name="properties"></a><span data-ttu-id="d1925-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d1925-107">Properties</span></span>
|<span data-ttu-id="d1925-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d1925-108">Property</span></span>|<span data-ttu-id="d1925-109">型</span><span class="sxs-lookup"><span data-stu-id="d1925-109">Type</span></span>|<span data-ttu-id="d1925-110">説明</span><span class="sxs-lookup"><span data-stu-id="d1925-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d1925-111">displayName</span><span class="sxs-lookup"><span data-stu-id="d1925-111">displayName</span></span>|<span data-ttu-id="d1925-112">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="d1925-112">String</span></span>|<span data-ttu-id="d1925-113">フォルダー ページの名前</span><span class="sxs-lookup"><span data-stu-id="d1925-113">Name of the folder page</span></span>|
|<span data-ttu-id="d1925-114">apps</span><span class="sxs-lookup"><span data-stu-id="d1925-114">apps</span></span>|<span data-ttu-id="d1925-115">[iosHomeScreenApp](../resources/intune-deviceconfig-ioshomescreenapp.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="d1925-115">[iosHomeScreenApp](../resources/intune-deviceconfig-ioshomescreenapp.md) collection</span></span>|<span data-ttu-id="d1925-116">フォルダー内のページに表示されるアプリの一覧。</span><span class="sxs-lookup"><span data-stu-id="d1925-116">A list of apps to appear on a page within a folder.</span></span> <span data-ttu-id="d1925-117">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="d1925-117">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d1925-118">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="d1925-118">Relationships</span></span>
<span data-ttu-id="d1925-119">なし</span><span class="sxs-lookup"><span data-stu-id="d1925-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d1925-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d1925-120">JSON Representation</span></span>
<span data-ttu-id="d1925-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="d1925-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosHomeScreenFolderPage"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosHomeScreenFolderPage",
  "displayName": "String",
  "apps": [
    {
      "@odata.type": "microsoft.graph.iosHomeScreenApp",
      "displayName": "String",
      "bundleID": "String"
    }
  ]
}
```




