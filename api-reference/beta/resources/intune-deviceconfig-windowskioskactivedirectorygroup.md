---
title: windowsKioskActiveDirectoryGroup リソースの種類
description: キオスクの構成の Azure ディレクトリ グループを識別するに使用するクラス
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 632396b727448032f198a54b97ba0a46b961abe5
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27955234"
---
# <a name="windowskioskactivedirectorygroup-resource-type"></a><span data-ttu-id="2905f-103">windowsKioskActiveDirectoryGroup リソースの種類</span><span class="sxs-lookup"><span data-stu-id="2905f-103">windowsKioskActiveDirectoryGroup resource type</span></span>

> <span data-ttu-id="2905f-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="2905f-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2905f-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2905f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2905f-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="2905f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2905f-107">キオスクの構成の Azure ディレクトリ グループを識別するに使用するクラス</span><span class="sxs-lookup"><span data-stu-id="2905f-107">The class used to identify an Azure Directory group for the kiosk configuration</span></span>

<span data-ttu-id="2905f-108">[WindowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="2905f-108">Inherits from [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span></span>

## <a name="properties"></a><span data-ttu-id="2905f-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2905f-109">Properties</span></span>
|<span data-ttu-id="2905f-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2905f-110">Property</span></span>|<span data-ttu-id="2905f-111">種類</span><span class="sxs-lookup"><span data-stu-id="2905f-111">Type</span></span>|<span data-ttu-id="2905f-112">説明</span><span class="sxs-lookup"><span data-stu-id="2905f-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2905f-113">グループ名</span><span class="sxs-lookup"><span data-stu-id="2905f-113">groupName</span></span>|<span data-ttu-id="2905f-114">String</span><span class="sxs-lookup"><span data-stu-id="2905f-114">String</span></span>|<span data-ttu-id="2905f-115">この構成にキオスクがロックアウトされている AD グループの名前</span><span class="sxs-lookup"><span data-stu-id="2905f-115">The name of the AD group that will be locked to this kiosk configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="2905f-116">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="2905f-116">Relationships</span></span>
<span data-ttu-id="2905f-117">なし</span><span class="sxs-lookup"><span data-stu-id="2905f-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="2905f-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2905f-118">JSON Representation</span></span>
<span data-ttu-id="2905f-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="2905f-119">Here is a JSON representation of the resource.</span></span>
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





