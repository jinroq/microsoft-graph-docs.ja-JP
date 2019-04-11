---
title: deviceManagementUserRightsSetting リソースの種類
description: ユーザー権限の設定を表します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2228e28b2edb3584a0861628644188d6fd54495b
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31802626"
---
# <a name="devicemanagementuserrightssetting-resource-type"></a><span data-ttu-id="76c07-103">deviceManagementUserRightsSetting リソースの種類</span><span class="sxs-lookup"><span data-stu-id="76c07-103">deviceManagementUserRightsSetting resource type</span></span>

> <span data-ttu-id="76c07-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="76c07-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="76c07-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="76c07-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="76c07-106">ユーザー権限の設定を表します。</span><span class="sxs-lookup"><span data-stu-id="76c07-106">Represents a user rights setting.</span></span>

## <a name="properties"></a><span data-ttu-id="76c07-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="76c07-107">Properties</span></span>
|<span data-ttu-id="76c07-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="76c07-108">Property</span></span>|<span data-ttu-id="76c07-109">型</span><span class="sxs-lookup"><span data-stu-id="76c07-109">Type</span></span>|<span data-ttu-id="76c07-110">説明</span><span class="sxs-lookup"><span data-stu-id="76c07-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="76c07-111">state</span><span class="sxs-lookup"><span data-stu-id="76c07-111">state</span></span>|[<span data-ttu-id="76c07-112">statemanagementsetting</span><span class="sxs-lookup"><span data-stu-id="76c07-112">stateManagementSetting</span></span>](../resources/intune-deviceconfig-statemanagementsetting.md)|<span data-ttu-id="76c07-113">このユーザー権限設定の現在の状態を表します。</span><span class="sxs-lookup"><span data-stu-id="76c07-113">Representing the current state of this user rights setting.</span></span> <span data-ttu-id="76c07-114">使用可能な値は、`notConfigured`、`blocked`、`allowed` です。</span><span class="sxs-lookup"><span data-stu-id="76c07-114">Possible values are: `notConfigured`, `blocked`, `allowed`.</span></span>|
|<span data-ttu-id="76c07-115">localusersorgroups</span><span class="sxs-lookup"><span data-stu-id="76c07-115">localUsersOrGroups</span></span>|<span data-ttu-id="76c07-116">[deviceManagementUserRightsLocalUserOrGroup](../resources/intune-deviceconfig-devicemanagementuserrightslocaluserorgroup.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="76c07-116">[deviceManagementUserRightsLocalUserOrGroup](../resources/intune-deviceconfig-devicemanagementuserrightslocaluserorgroup.md) collection</span></span>|<span data-ttu-id="76c07-117">この設定の状態が許可されている場合は、デバイスに設定されるローカルユーザーまたはグループのコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="76c07-117">Representing a collection of local users or groups which will be set on device if the state of this setting is Allowed.</span></span> <span data-ttu-id="76c07-118">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="76c07-118">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="76c07-119">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="76c07-119">Relationships</span></span>
<span data-ttu-id="76c07-120">なし</span><span class="sxs-lookup"><span data-stu-id="76c07-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="76c07-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="76c07-121">JSON Representation</span></span>
<span data-ttu-id="76c07-122">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="76c07-122">Here is a JSON representation of the resource.</span></span>
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





