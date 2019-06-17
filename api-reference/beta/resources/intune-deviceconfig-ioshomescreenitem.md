---
title: iosHomeScreenItem リソースの種類
description: IOS ホーム画面上のアイテムを表します
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 077c0eea7a4953d0cba3e9223a24fd9107f1b6c0
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34990254"
---
# <a name="ioshomescreenitem-resource-type"></a><span data-ttu-id="10fcd-103">iosHomeScreenItem リソースの種類</span><span class="sxs-lookup"><span data-stu-id="10fcd-103">iosHomeScreenItem resource type</span></span>

> <span data-ttu-id="10fcd-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="10fcd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="10fcd-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="10fcd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="10fcd-106">IOS ホーム画面上のアイテムを表します</span><span class="sxs-lookup"><span data-stu-id="10fcd-106">Represents an item on the iOS Home Screen</span></span>

## <a name="properties"></a><span data-ttu-id="10fcd-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="10fcd-107">Properties</span></span>
|<span data-ttu-id="10fcd-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="10fcd-108">Property</span></span>|<span data-ttu-id="10fcd-109">型</span><span class="sxs-lookup"><span data-stu-id="10fcd-109">Type</span></span>|<span data-ttu-id="10fcd-110">説明</span><span class="sxs-lookup"><span data-stu-id="10fcd-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="10fcd-111">displayName</span><span class="sxs-lookup"><span data-stu-id="10fcd-111">displayName</span></span>|<span data-ttu-id="10fcd-112">String</span><span class="sxs-lookup"><span data-stu-id="10fcd-112">String</span></span>|<span data-ttu-id="10fcd-113">アプリの名前</span><span class="sxs-lookup"><span data-stu-id="10fcd-113">Name of the app</span></span>|

## <a name="relationships"></a><span data-ttu-id="10fcd-114">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="10fcd-114">Relationships</span></span>
<span data-ttu-id="10fcd-115">なし</span><span class="sxs-lookup"><span data-stu-id="10fcd-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="10fcd-116">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="10fcd-116">JSON Representation</span></span>
<span data-ttu-id="10fcd-117">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="10fcd-117">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosHomeScreenItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosHomeScreenItem",
  "displayName": "String"
}
```





