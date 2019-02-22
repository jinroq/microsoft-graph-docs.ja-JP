---
title: windowsKioskActiveDirectoryGroup リソースの種類
description: キオスク構成の Azure ディレクトリグループを識別するために使用されるクラス
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e9f3345462583ab24850449d4a6178df7d5e3688
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30147076"
---
# <a name="windowskioskactivedirectorygroup-resource-type"></a><span data-ttu-id="4e3db-103">windowsKioskActiveDirectoryGroup リソースの種類</span><span class="sxs-lookup"><span data-stu-id="4e3db-103">windowsKioskActiveDirectoryGroup resource type</span></span>

> <span data-ttu-id="4e3db-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4e3db-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4e3db-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="4e3db-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4e3db-106">キオスク構成の Azure ディレクトリグループを識別するために使用されるクラス</span><span class="sxs-lookup"><span data-stu-id="4e3db-106">The class used to identify an Azure Directory group for the kiosk configuration</span></span>


<span data-ttu-id="4e3db-107">[windowskioskuser](../resources/intune-deviceconfig-windowskioskuser.md)からの継承</span><span class="sxs-lookup"><span data-stu-id="4e3db-107">Inherits from [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span></span>

## <a name="properties"></a><span data-ttu-id="4e3db-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4e3db-108">Properties</span></span>
|<span data-ttu-id="4e3db-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4e3db-109">Property</span></span>|<span data-ttu-id="4e3db-110">型</span><span class="sxs-lookup"><span data-stu-id="4e3db-110">Type</span></span>|<span data-ttu-id="4e3db-111">説明</span><span class="sxs-lookup"><span data-stu-id="4e3db-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4e3db-112">groupName</span><span class="sxs-lookup"><span data-stu-id="4e3db-112">groupName</span></span>|<span data-ttu-id="4e3db-113">String</span><span class="sxs-lookup"><span data-stu-id="4e3db-113">String</span></span>|<span data-ttu-id="4e3db-114">このキオスク構成にロックされる AD グループの名前</span><span class="sxs-lookup"><span data-stu-id="4e3db-114">The name of the AD group that will be locked to this kiosk configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="4e3db-115">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="4e3db-115">Relationships</span></span>
<span data-ttu-id="4e3db-116">なし</span><span class="sxs-lookup"><span data-stu-id="4e3db-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4e3db-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="4e3db-117">JSON Representation</span></span>
<span data-ttu-id="4e3db-118">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="4e3db-118">Here is a JSON representation of the resource.</span></span>
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




