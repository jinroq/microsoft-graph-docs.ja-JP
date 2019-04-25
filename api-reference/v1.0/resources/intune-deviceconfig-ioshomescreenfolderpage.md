---
title: iosHomeScreenFolderPage リソースの種類
description: ホーム画面上のアプリが含まれるフォルダー
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f00c67b7a0679d92ef6aac78bc0317e461dcd2f9
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32554640"
---
# <a name="ioshomescreenfolderpage-resource-type"></a><span data-ttu-id="2aeba-103">iosHomeScreenFolderPage リソースの種類</span><span class="sxs-lookup"><span data-stu-id="2aeba-103">iosHomeScreenFolderPage resource type</span></span>

> <span data-ttu-id="2aeba-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="2aeba-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2aeba-105">ホーム画面上のアプリが含まれるフォルダー</span><span class="sxs-lookup"><span data-stu-id="2aeba-105">A folder containing apps on the Home Screen</span></span>

## <a name="properties"></a><span data-ttu-id="2aeba-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2aeba-106">Properties</span></span>
|<span data-ttu-id="2aeba-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2aeba-107">Property</span></span>|<span data-ttu-id="2aeba-108">型</span><span class="sxs-lookup"><span data-stu-id="2aeba-108">Type</span></span>|<span data-ttu-id="2aeba-109">説明</span><span class="sxs-lookup"><span data-stu-id="2aeba-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2aeba-110">displayName</span><span class="sxs-lookup"><span data-stu-id="2aeba-110">displayName</span></span>|<span data-ttu-id="2aeba-111">String</span><span class="sxs-lookup"><span data-stu-id="2aeba-111">String</span></span>|<span data-ttu-id="2aeba-112">フォルダー ページの名前</span><span class="sxs-lookup"><span data-stu-id="2aeba-112">Name of the folder page</span></span>|
|<span data-ttu-id="2aeba-113">apps</span><span class="sxs-lookup"><span data-stu-id="2aeba-113">apps</span></span>|<span data-ttu-id="2aeba-114">[iosHomeScreenApp](../resources/intune-deviceconfig-ioshomescreenapp.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="2aeba-114">[iosHomeScreenApp](../resources/intune-deviceconfig-ioshomescreenapp.md) collection</span></span>|<span data-ttu-id="2aeba-115">フォルダー内のページに表示されるアプリの一覧。</span><span class="sxs-lookup"><span data-stu-id="2aeba-115">A list of apps to appear on a page within a folder.</span></span> <span data-ttu-id="2aeba-116">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="2aeba-116">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2aeba-117">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="2aeba-117">Relationships</span></span>
<span data-ttu-id="2aeba-118">なし</span><span class="sxs-lookup"><span data-stu-id="2aeba-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2aeba-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2aeba-119">JSON Representation</span></span>
<span data-ttu-id="2aeba-120">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="2aeba-120">Here is a JSON representation of the resource.</span></span>
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



