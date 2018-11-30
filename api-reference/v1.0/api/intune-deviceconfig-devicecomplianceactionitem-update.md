---
title: deviceComplianceActionItem の更新
description: deviceComplianceActionItem オブジェクトのプロパティを更新します。
ms.openlocfilehash: 8bebd6a37726266bc3519f9597f0968f0049318c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27020168"
---
# <a name="update-devicecomplianceactionitem"></a><span data-ttu-id="3989a-103">deviceComplianceActionItem の更新</span><span class="sxs-lookup"><span data-stu-id="3989a-103">Update deviceComplianceActionItem</span></span>

> <span data-ttu-id="3989a-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="3989a-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3989a-105">[deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="3989a-105">Update the properties of a [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3989a-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="3989a-106">Prerequisites</span></span>
<span data-ttu-id="3989a-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3989a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3989a-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3989a-109">Permission type</span></span>|<span data-ttu-id="3989a-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="3989a-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3989a-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3989a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="3989a-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3989a-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3989a-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3989a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3989a-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3989a-114">Not supported.</span></span>|
|<span data-ttu-id="3989a-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3989a-115">Application</span></span>|<span data-ttu-id="3989a-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3989a-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3989a-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3989a-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations/{deviceComplianceActionItemId}
```

## <a name="request-headers"></a><span data-ttu-id="3989a-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3989a-118">Request headers</span></span>
|<span data-ttu-id="3989a-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3989a-119">Header</span></span>|<span data-ttu-id="3989a-120">値</span><span class="sxs-lookup"><span data-stu-id="3989a-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3989a-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="3989a-121">Authorization</span></span>|<span data-ttu-id="3989a-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="3989a-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3989a-123">Accept</span><span class="sxs-lookup"><span data-stu-id="3989a-123">Accept</span></span>|<span data-ttu-id="3989a-124">application/json</span><span class="sxs-lookup"><span data-stu-id="3989a-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3989a-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="3989a-125">Request body</span></span>
<span data-ttu-id="3989a-126">要求本文で、[deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="3989a-126">In the request body, supply a JSON representation for the [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>

<span data-ttu-id="3989a-127">次の表に、[deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="3989a-127">The following table shows the properties that are required when you create the [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md).</span></span>

|<span data-ttu-id="3989a-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3989a-128">Property</span></span>|<span data-ttu-id="3989a-129">型</span><span class="sxs-lookup"><span data-stu-id="3989a-129">Type</span></span>|<span data-ttu-id="3989a-130">説明</span><span class="sxs-lookup"><span data-stu-id="3989a-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3989a-131">id</span><span class="sxs-lookup"><span data-stu-id="3989a-131">id</span></span>|<span data-ttu-id="3989a-132">String</span><span class="sxs-lookup"><span data-stu-id="3989a-132">String</span></span>|<span data-ttu-id="3989a-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="3989a-133">Key of the entity.</span></span>|
|<span data-ttu-id="3989a-134">gracePeriodHours</span><span class="sxs-lookup"><span data-stu-id="3989a-134">gracePeriodHours</span></span>|<span data-ttu-id="3989a-135">Int32</span><span class="sxs-lookup"><span data-stu-id="3989a-135">Int32</span></span>|<span data-ttu-id="3989a-136">アクションが実行されるまでの待機時間。</span><span class="sxs-lookup"><span data-stu-id="3989a-136">Number of hours to wait till the action will be enforced.</span></span> <span data-ttu-id="3989a-137">有効な値は 0 から 8760 までです</span><span class="sxs-lookup"><span data-stu-id="3989a-137">Valid values 0 to 8760</span></span>|
|<span data-ttu-id="3989a-138">actionType</span><span class="sxs-lookup"><span data-stu-id="3989a-138">actionType</span></span>|[<span data-ttu-id="3989a-139">deviceComplianceActionType</span><span class="sxs-lookup"><span data-stu-id="3989a-139">deviceComplianceActionType</span></span>](../resources/intune-deviceconfig-devicecomplianceactiontype.md)|<span data-ttu-id="3989a-140">実行するアクションです。</span><span class="sxs-lookup"><span data-stu-id="3989a-140">What action to take.</span></span> <span data-ttu-id="3989a-141">可能な値は、`noAction`、`notification`、`block`、`retire`、`wipe`、`removeResourceAccessProfiles`、`pushNotification` です。</span><span class="sxs-lookup"><span data-stu-id="3989a-141">Possible values are: `noAction`, `notification`, `block`, `retire`, `wipe`, `removeResourceAccessProfiles`, `pushNotification`.</span></span>|
|<span data-ttu-id="3989a-142">notificationTemplateId</span><span class="sxs-lookup"><span data-stu-id="3989a-142">notificationTemplateId</span></span>|<span data-ttu-id="3989a-143">String</span><span class="sxs-lookup"><span data-stu-id="3989a-143">String</span></span>|<span data-ttu-id="3989a-144">使用する通知メッセージ テンプレート</span><span class="sxs-lookup"><span data-stu-id="3989a-144">What notification Message template to use</span></span>|
|<span data-ttu-id="3989a-145">notificationMessageCCList</span><span class="sxs-lookup"><span data-stu-id="3989a-145">notificationMessageCCList</span></span>|<span data-ttu-id="3989a-146">String コレクション</span><span class="sxs-lookup"><span data-stu-id="3989a-146">String collection</span></span>|<span data-ttu-id="3989a-147">この通知メッセージの CC に設定するグループ ID のリスト。</span><span class="sxs-lookup"><span data-stu-id="3989a-147">A list of group IDs to speicify who to CC this notification message to.</span></span>|



## <a name="response"></a><span data-ttu-id="3989a-148">応答</span><span class="sxs-lookup"><span data-stu-id="3989a-148">Response</span></span>
<span data-ttu-id="3989a-149">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="3989a-149">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3989a-150">例</span><span class="sxs-lookup"><span data-stu-id="3989a-150">Example</span></span>
### <a name="request"></a><span data-ttu-id="3989a-151">要求</span><span class="sxs-lookup"><span data-stu-id="3989a-151">Request</span></span>
<span data-ttu-id="3989a-152">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="3989a-152">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations/{deviceComplianceActionItemId}
Content-type: application/json
Content-length: 271

{
  "@odata.type": "#microsoft.graph.deviceComplianceActionItem",
  "gracePeriodHours": 0,
  "actionType": "notification",
  "notificationTemplateId": "Notification Template Id value",
  "notificationMessageCCList": [
    "Notification Message CCList value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="3989a-153">応答</span><span class="sxs-lookup"><span data-stu-id="3989a-153">Response</span></span>
<span data-ttu-id="3989a-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="3989a-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



