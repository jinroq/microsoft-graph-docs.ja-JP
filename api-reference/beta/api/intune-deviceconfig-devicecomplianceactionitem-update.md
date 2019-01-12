---
title: deviceComplianceActionItem の更新
description: deviceComplianceActionItem オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: c117c13d9519f3a81bd98096304bc2477ac31933
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27942410"
---
# <a name="update-devicecomplianceactionitem"></a><span data-ttu-id="7cd9e-103">deviceComplianceActionItem の更新</span><span class="sxs-lookup"><span data-stu-id="7cd9e-103">Update deviceComplianceActionItem</span></span>

> <span data-ttu-id="7cd9e-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="7cd9e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7cd9e-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7cd9e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7cd9e-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="7cd9e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7cd9e-107">[deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="7cd9e-107">Update the properties of a [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7cd9e-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="7cd9e-108">Prerequisites</span></span>
<span data-ttu-id="7cd9e-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7cd9e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7cd9e-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7cd9e-111">Permission type</span></span>|<span data-ttu-id="7cd9e-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="7cd9e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7cd9e-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7cd9e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7cd9e-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7cd9e-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7cd9e-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7cd9e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7cd9e-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7cd9e-116">Not supported.</span></span>|
|<span data-ttu-id="7cd9e-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7cd9e-117">Application</span></span>|<span data-ttu-id="7cd9e-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7cd9e-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7cd9e-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7cd9e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations/{deviceComplianceActionItemId}
```

## <a name="request-headers"></a><span data-ttu-id="7cd9e-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7cd9e-120">Request headers</span></span>
|<span data-ttu-id="7cd9e-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7cd9e-121">Header</span></span>|<span data-ttu-id="7cd9e-122">値</span><span class="sxs-lookup"><span data-stu-id="7cd9e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7cd9e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7cd9e-123">Authorization</span></span>|<span data-ttu-id="7cd9e-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="7cd9e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7cd9e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="7cd9e-125">Accept</span></span>|<span data-ttu-id="7cd9e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7cd9e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7cd9e-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="7cd9e-127">Request body</span></span>
<span data-ttu-id="7cd9e-128">要求本文で、[deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="7cd9e-128">In the request body, supply a JSON representation for the [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>

<span data-ttu-id="7cd9e-129">次の表に、[deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="7cd9e-129">The following table shows the properties that are required when you create the [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md).</span></span>

|<span data-ttu-id="7cd9e-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7cd9e-130">Property</span></span>|<span data-ttu-id="7cd9e-131">型</span><span class="sxs-lookup"><span data-stu-id="7cd9e-131">Type</span></span>|<span data-ttu-id="7cd9e-132">説明</span><span class="sxs-lookup"><span data-stu-id="7cd9e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7cd9e-133">ID</span><span class="sxs-lookup"><span data-stu-id="7cd9e-133">id</span></span>|<span data-ttu-id="7cd9e-134">String</span><span class="sxs-lookup"><span data-stu-id="7cd9e-134">String</span></span>|<span data-ttu-id="7cd9e-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="7cd9e-135">Key of the entity.</span></span>|
|<span data-ttu-id="7cd9e-136">gracePeriodHours</span><span class="sxs-lookup"><span data-stu-id="7cd9e-136">gracePeriodHours</span></span>|<span data-ttu-id="7cd9e-137">Int32</span><span class="sxs-lookup"><span data-stu-id="7cd9e-137">Int32</span></span>|<span data-ttu-id="7cd9e-138">アクションが実行されるまでの待機時間。</span><span class="sxs-lookup"><span data-stu-id="7cd9e-138">Number of hours to wait till the action will be enforced.</span></span> <span data-ttu-id="7cd9e-139">有効な値は 0 から 8760 までです</span><span class="sxs-lookup"><span data-stu-id="7cd9e-139">Valid values 0 to 8760</span></span>|
|<span data-ttu-id="7cd9e-140">actionType</span><span class="sxs-lookup"><span data-stu-id="7cd9e-140">actionType</span></span>|[<span data-ttu-id="7cd9e-141">deviceComplianceActionType</span><span class="sxs-lookup"><span data-stu-id="7cd9e-141">deviceComplianceActionType</span></span>](../resources/intune-deviceconfig-devicecomplianceactiontype.md)|<span data-ttu-id="7cd9e-142">実行するアクションです。</span><span class="sxs-lookup"><span data-stu-id="7cd9e-142">What action to take.</span></span> <span data-ttu-id="7cd9e-143">可能な値は、`noAction`、`notification`、`block`、`retire`、`wipe`、`removeResourceAccessProfiles`、`pushNotification`、`remoteLock` です。</span><span class="sxs-lookup"><span data-stu-id="7cd9e-143">Possible values are: `noAction`, `notification`, `block`, `retire`, `wipe`, `removeResourceAccessProfiles`, `pushNotification`, `remoteLock`.</span></span>|
|<span data-ttu-id="7cd9e-144">notificationTemplateId</span><span class="sxs-lookup"><span data-stu-id="7cd9e-144">notificationTemplateId</span></span>|<span data-ttu-id="7cd9e-145">String</span><span class="sxs-lookup"><span data-stu-id="7cd9e-145">String</span></span>|<span data-ttu-id="7cd9e-146">使用する通知メッセージ テンプレート</span><span class="sxs-lookup"><span data-stu-id="7cd9e-146">What notification Message template to use</span></span>|
|<span data-ttu-id="7cd9e-147">notificationMessageCCList</span><span class="sxs-lookup"><span data-stu-id="7cd9e-147">notificationMessageCCList</span></span>|<span data-ttu-id="7cd9e-148">String コレクション</span><span class="sxs-lookup"><span data-stu-id="7cd9e-148">String collection</span></span>|<span data-ttu-id="7cd9e-149">この通知メッセージの CC に設定するグループ ID のリスト。</span><span class="sxs-lookup"><span data-stu-id="7cd9e-149">A list of group IDs to speicify who to CC this notification message to.</span></span>|



## <a name="response"></a><span data-ttu-id="7cd9e-150">応答</span><span class="sxs-lookup"><span data-stu-id="7cd9e-150">Response</span></span>
<span data-ttu-id="7cd9e-151">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="7cd9e-151">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7cd9e-152">例</span><span class="sxs-lookup"><span data-stu-id="7cd9e-152">Example</span></span>
### <a name="request"></a><span data-ttu-id="7cd9e-153">要求</span><span class="sxs-lookup"><span data-stu-id="7cd9e-153">Request</span></span>
<span data-ttu-id="7cd9e-154">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="7cd9e-154">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations/{deviceComplianceActionItemId}
Content-type: application/json
Content-length: 206

{
  "gracePeriodHours": 0,
  "actionType": "notification",
  "notificationTemplateId": "Notification Template Id value",
  "notificationMessageCCList": [
    "Notification Message CCList value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="7cd9e-155">応答</span><span class="sxs-lookup"><span data-stu-id="7cd9e-155">Response</span></span>
<span data-ttu-id="7cd9e-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="7cd9e-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 320

{
  "@odata.type": "#microsoft.graph.deviceComplianceActionItem",
  "id": "e01a1893-1893-e01a-9318-1ae093181ae0",
  "gracePeriodHours": 0,
  "actionType": "notification",
  "notificationTemplateId": "Notification Template Id value",
  "notificationMessageCCList": [
    "Notification Message CCList value"
  ]
}
```





