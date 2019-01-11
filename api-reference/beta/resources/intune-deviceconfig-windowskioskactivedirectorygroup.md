---
title: windowsKioskActiveDirectoryGroup リソースの種類
description: キオスクの構成の Azure ディレクトリ グループを識別するに使用するクラス
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: dc9db9aa120411c423492efa162973e33cc4c303
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27850527"
---
# <a name="windowskioskactivedirectorygroup-resource-type"></a><span data-ttu-id="cae1e-103">windowsKioskActiveDirectoryGroup リソースの種類</span><span class="sxs-lookup"><span data-stu-id="cae1e-103">windowsKioskActiveDirectoryGroup resource type</span></span>

> <span data-ttu-id="cae1e-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="cae1e-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cae1e-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cae1e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cae1e-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="cae1e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cae1e-107">キオスクの構成の Azure ディレクトリ グループを識別するに使用するクラス</span><span class="sxs-lookup"><span data-stu-id="cae1e-107">The class used to identify an Azure Directory group for the kiosk configuration</span></span>

<span data-ttu-id="cae1e-108">[WindowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="cae1e-108">Inherits from [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span></span>

## <a name="properties"></a><span data-ttu-id="cae1e-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cae1e-109">Properties</span></span>
|<span data-ttu-id="cae1e-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cae1e-110">Property</span></span>|<span data-ttu-id="cae1e-111">種類</span><span class="sxs-lookup"><span data-stu-id="cae1e-111">Type</span></span>|<span data-ttu-id="cae1e-112">説明</span><span class="sxs-lookup"><span data-stu-id="cae1e-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cae1e-113">グループ名</span><span class="sxs-lookup"><span data-stu-id="cae1e-113">groupName</span></span>|<span data-ttu-id="cae1e-114">String</span><span class="sxs-lookup"><span data-stu-id="cae1e-114">String</span></span>|<span data-ttu-id="cae1e-115">この構成にキオスクがロックアウトされている AD グループの名前</span><span class="sxs-lookup"><span data-stu-id="cae1e-115">The name of the AD group that will be locked to this kiosk configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="cae1e-116">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="cae1e-116">Relationships</span></span>
<span data-ttu-id="cae1e-117">なし</span><span class="sxs-lookup"><span data-stu-id="cae1e-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="cae1e-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="cae1e-118">JSON Representation</span></span>
<span data-ttu-id="cae1e-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="cae1e-119">Here is a JSON representation of the resource.</span></span>
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





