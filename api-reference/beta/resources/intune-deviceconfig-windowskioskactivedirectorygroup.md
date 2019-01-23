---
title: windowsKioskActiveDirectoryGroup リソースの種類
description: キオスクの構成の Azure ディレクトリ グループを識別するに使用するクラス
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 88b151b856809247cfa6e5e211cc45c6f33c4c53
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29415713"
---
# <a name="windowskioskactivedirectorygroup-resource-type"></a><span data-ttu-id="5a9fb-103">windowsKioskActiveDirectoryGroup リソースの種類</span><span class="sxs-lookup"><span data-stu-id="5a9fb-103">windowsKioskActiveDirectoryGroup resource type</span></span>

> <span data-ttu-id="5a9fb-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="5a9fb-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="5a9fb-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5a9fb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5a9fb-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="5a9fb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5a9fb-107">キオスクの構成の Azure ディレクトリ グループを識別するに使用するクラス</span><span class="sxs-lookup"><span data-stu-id="5a9fb-107">The class used to identify an Azure Directory group for the kiosk configuration</span></span>


<span data-ttu-id="5a9fb-108">[WindowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="5a9fb-108">Inherits from [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span></span>

## <a name="properties"></a><span data-ttu-id="5a9fb-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5a9fb-109">Properties</span></span>
|<span data-ttu-id="5a9fb-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5a9fb-110">Property</span></span>|<span data-ttu-id="5a9fb-111">型</span><span class="sxs-lookup"><span data-stu-id="5a9fb-111">Type</span></span>|<span data-ttu-id="5a9fb-112">説明</span><span class="sxs-lookup"><span data-stu-id="5a9fb-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5a9fb-113">グループ名</span><span class="sxs-lookup"><span data-stu-id="5a9fb-113">groupName</span></span>|<span data-ttu-id="5a9fb-114">String</span><span class="sxs-lookup"><span data-stu-id="5a9fb-114">String</span></span>|<span data-ttu-id="5a9fb-115">この構成にキオスクがロックアウトされている AD グループの名前</span><span class="sxs-lookup"><span data-stu-id="5a9fb-115">The name of the AD group that will be locked to this kiosk configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="5a9fb-116">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="5a9fb-116">Relationships</span></span>
<span data-ttu-id="5a9fb-117">なし</span><span class="sxs-lookup"><span data-stu-id="5a9fb-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5a9fb-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="5a9fb-118">JSON Representation</span></span>
<span data-ttu-id="5a9fb-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="5a9fb-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskActiveDirectoryGroup"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskActiveDirectoryGroup",
  "groupName": "String"
}
```




