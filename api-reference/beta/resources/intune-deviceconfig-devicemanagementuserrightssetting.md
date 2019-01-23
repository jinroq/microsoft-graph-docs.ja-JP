---
title: deviceManagementUserRightsSetting リソースの種類
description: ユーザー権限の設定を表します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 35e6ec1a5faa5556a0e113df145d718c488b1669
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29415055"
---
# <a name="devicemanagementuserrightssetting-resource-type"></a><span data-ttu-id="42fb5-103">deviceManagementUserRightsSetting リソースの種類</span><span class="sxs-lookup"><span data-stu-id="42fb5-103">deviceManagementUserRightsSetting resource type</span></span>

> <span data-ttu-id="42fb5-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="42fb5-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="42fb5-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="42fb5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="42fb5-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="42fb5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="42fb5-107">ユーザー権限の設定を表します。</span><span class="sxs-lookup"><span data-stu-id="42fb5-107">Represents a user rights setting.</span></span>

## <a name="properties"></a><span data-ttu-id="42fb5-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="42fb5-108">Properties</span></span>
|<span data-ttu-id="42fb5-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="42fb5-109">Property</span></span>|<span data-ttu-id="42fb5-110">型</span><span class="sxs-lookup"><span data-stu-id="42fb5-110">Type</span></span>|<span data-ttu-id="42fb5-111">説明</span><span class="sxs-lookup"><span data-stu-id="42fb5-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="42fb5-112">state</span><span class="sxs-lookup"><span data-stu-id="42fb5-112">state</span></span>|[<span data-ttu-id="42fb5-113">stateManagementSetting</span><span class="sxs-lookup"><span data-stu-id="42fb5-113">stateManagementSetting</span></span>](../resources/intune-deviceconfig-statemanagementsetting.md)|<span data-ttu-id="42fb5-114">このユーザーの現在の状態を表す権限を設定します。</span><span class="sxs-lookup"><span data-stu-id="42fb5-114">Representing the current state of this user rights setting.</span></span> <span data-ttu-id="42fb5-115">可能な値は、`notConfigured`、`blocked`、`allowed` です。</span><span class="sxs-lookup"><span data-stu-id="42fb5-115">Possible values are: `notConfigured`, `blocked`, `allowed`.</span></span>|
|<span data-ttu-id="42fb5-116">localUsersOrGroups</span><span class="sxs-lookup"><span data-stu-id="42fb5-116">localUsersOrGroups</span></span>|<span data-ttu-id="42fb5-117">[deviceManagementUserRightsLocalUserOrGroup](../resources/intune-deviceconfig-devicemanagementuserrightslocaluserorgroup.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="42fb5-117">[deviceManagementUserRightsLocalUserOrGroup](../resources/intune-deviceconfig-devicemanagementuserrightslocaluserorgroup.md) collection</span></span>|<span data-ttu-id="42fb5-118">ローカル ユーザーまたはグループはこの設定の状態が許可されている場合に、デバイスの設定のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="42fb5-118">Representing a collection of local users or groups which will be set on device if the state of this setting is Allowed.</span></span> <span data-ttu-id="42fb5-119">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="42fb5-119">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="42fb5-120">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="42fb5-120">Relationships</span></span>
<span data-ttu-id="42fb5-121">なし</span><span class="sxs-lookup"><span data-stu-id="42fb5-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="42fb5-122">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="42fb5-122">JSON Representation</span></span>
<span data-ttu-id="42fb5-123">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="42fb5-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementUserRightsSetting"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementUserRightsSetting",
  "state": "String",
  "localUsersOrGroups": [
    {
      "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
      "name": "String",
      "description": "String",
      "securityIdentifier": "String"
    }
  ]
}
```




