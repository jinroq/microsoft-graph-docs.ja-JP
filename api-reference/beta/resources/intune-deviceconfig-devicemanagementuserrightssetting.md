---
title: deviceManagementUserRightsSetting リソースの種類
description: ユーザー権限の設定を表します。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: b12dc0c1c682b59ef741b3d49083fd0739d27abb
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27844808"
---
# <a name="devicemanagementuserrightssetting-resource-type"></a><span data-ttu-id="6c7d0-103">deviceManagementUserRightsSetting リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6c7d0-103">deviceManagementUserRightsSetting resource type</span></span>

> <span data-ttu-id="6c7d0-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="6c7d0-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6c7d0-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6c7d0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6c7d0-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="6c7d0-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6c7d0-107">ユーザー権限の設定を表します。</span><span class="sxs-lookup"><span data-stu-id="6c7d0-107">Represents a user rights setting.</span></span>
## <a name="properties"></a><span data-ttu-id="6c7d0-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6c7d0-108">Properties</span></span>
|<span data-ttu-id="6c7d0-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6c7d0-109">Property</span></span>|<span data-ttu-id="6c7d0-110">種類</span><span class="sxs-lookup"><span data-stu-id="6c7d0-110">Type</span></span>|<span data-ttu-id="6c7d0-111">説明</span><span class="sxs-lookup"><span data-stu-id="6c7d0-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6c7d0-112">state</span><span class="sxs-lookup"><span data-stu-id="6c7d0-112">state</span></span>|[<span data-ttu-id="6c7d0-113">stateManagementSetting</span><span class="sxs-lookup"><span data-stu-id="6c7d0-113">stateManagementSetting</span></span>](../resources/intune-deviceconfig-statemanagementsetting.md)|<span data-ttu-id="6c7d0-114">このユーザーの現在の状態を表す権限を設定します。</span><span class="sxs-lookup"><span data-stu-id="6c7d0-114">Representing the current state of this user rights setting.</span></span> <span data-ttu-id="6c7d0-115">可能な値は、`notConfigured`、`blocked`、`allowed` です。</span><span class="sxs-lookup"><span data-stu-id="6c7d0-115">Possible values are: `notConfigured`, `blocked`, `allowed`.</span></span>|
|<span data-ttu-id="6c7d0-116">localUsersOrGroups</span><span class="sxs-lookup"><span data-stu-id="6c7d0-116">localUsersOrGroups</span></span>|<span data-ttu-id="6c7d0-117">[deviceManagementUserRightsLocalUserOrGroup](../resources/intune-deviceconfig-devicemanagementuserrightslocaluserorgroup.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="6c7d0-117">[deviceManagementUserRightsLocalUserOrGroup](../resources/intune-deviceconfig-devicemanagementuserrightslocaluserorgroup.md) collection</span></span>|<span data-ttu-id="6c7d0-118">ローカル ユーザーまたはグループはこの設定の状態が許可されている場合に、デバイスの設定のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="6c7d0-118">Representing a collection of local users or groups which will be set on device if the state of this setting is Allowed.</span></span> <span data-ttu-id="6c7d0-119">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="6c7d0-119">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6c7d0-120">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="6c7d0-120">Relationships</span></span>
<span data-ttu-id="6c7d0-121">なし</span><span class="sxs-lookup"><span data-stu-id="6c7d0-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="6c7d0-122">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6c7d0-122">JSON Representation</span></span>
<span data-ttu-id="6c7d0-123">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="6c7d0-123">Here is a JSON representation of the resource.</span></span>
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





