---
title: iosHomeScreenFolder リソースの種類
description: ホーム画面上のアプリのページが含まれるフォルダー
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9526e51b4fa69f0332922481c53648eb7d574c10
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32521629"
---
# <a name="ioshomescreenfolder-resource-type"></a><span data-ttu-id="a4790-103">iosHomeScreenFolder リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a4790-103">iosHomeScreenFolder resource type</span></span>

> <span data-ttu-id="a4790-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a4790-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a4790-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="a4790-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a4790-106">ホーム画面上のアプリのページが含まれるフォルダー</span><span class="sxs-lookup"><span data-stu-id="a4790-106">A folder containing pages of apps on the Home Screen</span></span>


<span data-ttu-id="a4790-107">[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="a4790-107">Inherits from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="a4790-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a4790-108">Properties</span></span>
|<span data-ttu-id="a4790-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a4790-109">Property</span></span>|<span data-ttu-id="a4790-110">型</span><span class="sxs-lookup"><span data-stu-id="a4790-110">Type</span></span>|<span data-ttu-id="a4790-111">説明</span><span class="sxs-lookup"><span data-stu-id="a4790-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a4790-112">displayName</span><span class="sxs-lookup"><span data-stu-id="a4790-112">displayName</span></span>|<span data-ttu-id="a4790-113">String</span><span class="sxs-lookup"><span data-stu-id="a4790-113">String</span></span>|<span data-ttu-id="a4790-114">アプリの名前。[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) から継承</span><span class="sxs-lookup"><span data-stu-id="a4790-114">Name of the app Inherited from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>|
|<span data-ttu-id="a4790-115">pages</span><span class="sxs-lookup"><span data-stu-id="a4790-115">pages</span></span>|<span data-ttu-id="a4790-116">[iosHomeScreenFolderPage](../resources/intune-deviceconfig-ioshomescreenfolderpage.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="a4790-116">[iosHomeScreenFolderPage](../resources/intune-deviceconfig-ioshomescreenfolderpage.md) collection</span></span>|<span data-ttu-id="a4790-117">アプリケーションの種類にする必要がある、ホーム画面レイアウト アイコンで構成されるページ。</span><span class="sxs-lookup"><span data-stu-id="a4790-117">Pages of Home Screen Layout Icons which must be Application Type.</span></span> <span data-ttu-id="a4790-118">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="a4790-118">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a4790-119">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="a4790-119">Relationships</span></span>
<span data-ttu-id="a4790-120">なし</span><span class="sxs-lookup"><span data-stu-id="a4790-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a4790-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a4790-121">JSON Representation</span></span>
<span data-ttu-id="a4790-122">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="a4790-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosHomeScreenFolder"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosHomeScreenFolder",
  "displayName": "String",
  "pages": [
    {
      "@odata.type": "microsoft.graph.iosHomeScreenFolderPage",
      "displayName": "String",
      "apps": [
        {
          "@odata.type": "microsoft.graph.iosHomeScreenApp",
          "displayName": "String",
          "bundleID": "String"
        }
      ]
    }
  ]
}
```





