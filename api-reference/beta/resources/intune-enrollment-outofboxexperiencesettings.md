---
title: outOfBoxExperienceSettings リソースの種類
description: ボックスの設定が発生します。
author: tfitzmac
ms.openlocfilehash: 545fbe5c27063397a4d08c40729227804ebfc56d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27308408"
---
# <a name="outofboxexperiencesettings-resource-type"></a><span data-ttu-id="1b49d-103">outOfBoxExperienceSettings リソースの種類</span><span class="sxs-lookup"><span data-stu-id="1b49d-103">outOfBoxExperienceSettings resource type</span></span>

> <span data-ttu-id="1b49d-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="1b49d-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1b49d-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1b49d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1b49d-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="1b49d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1b49d-107">ボックスの設定が発生します。</span><span class="sxs-lookup"><span data-stu-id="1b49d-107">Out of box experience setting</span></span>
## <a name="properties"></a><span data-ttu-id="1b49d-108">Properties</span><span class="sxs-lookup"><span data-stu-id="1b49d-108">Properties</span></span>
|<span data-ttu-id="1b49d-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1b49d-109">Property</span></span>|<span data-ttu-id="1b49d-110">種類</span><span class="sxs-lookup"><span data-stu-id="1b49d-110">Type</span></span>|<span data-ttu-id="1b49d-111">説明</span><span class="sxs-lookup"><span data-stu-id="1b49d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1b49d-112">hidePrivacySettings</span><span class="sxs-lookup"><span data-stu-id="1b49d-112">hidePrivacySettings</span></span>|<span data-ttu-id="1b49d-113">ブール型</span><span class="sxs-lookup"><span data-stu-id="1b49d-113">Boolean</span></span>|<span data-ttu-id="1b49d-114">ユーザーのプライバシー設定の表示と非表示を切り替える</span><span class="sxs-lookup"><span data-stu-id="1b49d-114">Show or hide privacy settings to user</span></span>|
|<span data-ttu-id="1b49d-115">hideEULA</span><span class="sxs-lookup"><span data-stu-id="1b49d-115">hideEULA</span></span>|<span data-ttu-id="1b49d-116">ブール型</span><span class="sxs-lookup"><span data-stu-id="1b49d-116">Boolean</span></span>|<span data-ttu-id="1b49d-117">ユーザーに使用許諾契約書の表示と非表示を切り替える</span><span class="sxs-lookup"><span data-stu-id="1b49d-117">Show or hide EULA to user</span></span>|
|<span data-ttu-id="1b49d-118">userType</span><span class="sxs-lookup"><span data-stu-id="1b49d-118">userType</span></span>|[<span data-ttu-id="1b49d-119">windowsUserType</span><span class="sxs-lookup"><span data-stu-id="1b49d-119">windowsUserType</span></span>](../resources/intune-enrollment-windowsusertype.md)|<span data-ttu-id="1b49d-120">ユーザーの種類です。</span><span class="sxs-lookup"><span data-stu-id="1b49d-120">Type of user.</span></span> <span data-ttu-id="1b49d-121">使用可能な値は、`administrator`、`standard` です。</span><span class="sxs-lookup"><span data-stu-id="1b49d-121">Possible values are: `administrator`, `standard`.</span></span>|
|<span data-ttu-id="1b49d-122">deviceUsageType</span><span class="sxs-lookup"><span data-stu-id="1b49d-122">deviceUsageType</span></span>|[<span data-ttu-id="1b49d-123">windowsDeviceUsageType</span><span class="sxs-lookup"><span data-stu-id="1b49d-123">windowsDeviceUsageType</span></span>](../resources/intune-enrollment-windowsdeviceusagetype.md)|<span data-ttu-id="1b49d-124">AAD の結合の認証の種類です。</span><span class="sxs-lookup"><span data-stu-id="1b49d-124">AAD join authentication type.</span></span> <span data-ttu-id="1b49d-125">使用可能な値は、`singleUser`、`shared` です。</span><span class="sxs-lookup"><span data-stu-id="1b49d-125">Possible values are: `singleUser`, `shared`.</span></span>|
|<span data-ttu-id="1b49d-126">skipKeyboardSelectionPage</span><span class="sxs-lookup"><span data-stu-id="1b49d-126">skipKeyboardSelectionPage</span></span>|<span data-ttu-id="1b49d-127">ブール型</span><span class="sxs-lookup"><span data-stu-id="1b49d-127">Boolean</span></span>|<span data-ttu-id="1b49d-128">かどうか、セット、キーボードの選択をスキップするページの言語と地域が設定されている場合</span><span class="sxs-lookup"><span data-stu-id="1b49d-128">If set, then skip the keyboard selection page if Language and Region are set</span></span>|
|<span data-ttu-id="1b49d-129">hideEscapeLink</span><span class="sxs-lookup"><span data-stu-id="1b49d-129">hideEscapeLink</span></span>|<span data-ttu-id="1b49d-130">ブール型</span><span class="sxs-lookup"><span data-stu-id="1b49d-130">Boolean</span></span>|<span data-ttu-id="1b49d-131">ユーザーでは、true に設定を別のアカウントでのサインインの会社経由で起動できない場合</span><span class="sxs-lookup"><span data-stu-id="1b49d-131">If set to true, then the user can't start over with different account, on company sign-in</span></span>|

## <a name="relationships"></a><span data-ttu-id="1b49d-132">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="1b49d-132">Relationships</span></span>
<span data-ttu-id="1b49d-133">なし</span><span class="sxs-lookup"><span data-stu-id="1b49d-133">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="1b49d-134">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="1b49d-134">JSON Representation</span></span>
<span data-ttu-id="1b49d-135">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="1b49d-135">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.outOfBoxExperienceSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.outOfBoxExperienceSettings",
  "hidePrivacySettings": true,
  "hideEULA": true,
  "userType": "String",
  "deviceUsageType": "String",
  "skipKeyboardSelectionPage": true,
  "hideEscapeLink": true
}
```





