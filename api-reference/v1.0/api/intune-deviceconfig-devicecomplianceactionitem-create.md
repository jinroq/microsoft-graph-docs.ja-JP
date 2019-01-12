---
title: deviceComplianceActionItem の作成
description: 新しい deviceComplianceActionItem オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: cd7cb91d6dde4755f27bdc28b3fb1c0c8804a800
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27972062"
---
# <a name="create-devicecomplianceactionitem"></a><span data-ttu-id="fa73b-103">deviceComplianceActionItem の作成</span><span class="sxs-lookup"><span data-stu-id="fa73b-103">Create deviceComplianceActionItem</span></span>

> <span data-ttu-id="fa73b-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="fa73b-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fa73b-105">新しい [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="fa73b-105">Create a new [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="fa73b-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="fa73b-106">Prerequisites</span></span>
<span data-ttu-id="fa73b-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fa73b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fa73b-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="fa73b-109">Permission type</span></span>|<span data-ttu-id="fa73b-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="fa73b-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fa73b-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="fa73b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="fa73b-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fa73b-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="fa73b-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="fa73b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fa73b-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fa73b-114">Not supported.</span></span>|
|<span data-ttu-id="fa73b-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="fa73b-115">Application</span></span>|<span data-ttu-id="fa73b-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fa73b-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fa73b-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="fa73b-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="fa73b-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fa73b-118">Request headers</span></span>
|<span data-ttu-id="fa73b-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fa73b-119">Header</span></span>|<span data-ttu-id="fa73b-120">値</span><span class="sxs-lookup"><span data-stu-id="fa73b-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fa73b-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="fa73b-121">Authorization</span></span>|<span data-ttu-id="fa73b-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="fa73b-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fa73b-123">Accept</span><span class="sxs-lookup"><span data-stu-id="fa73b-123">Accept</span></span>|<span data-ttu-id="fa73b-124">application/json</span><span class="sxs-lookup"><span data-stu-id="fa73b-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fa73b-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="fa73b-125">Request body</span></span>
<span data-ttu-id="fa73b-126">要求本文で、deviceComplianceActionItem オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="fa73b-126">In the request body, supply a JSON representation for the deviceComplianceActionItem object.</span></span>

<span data-ttu-id="fa73b-127">次の表に、deviceComplianceActionItem の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="fa73b-127">The following table shows the properties that are required when you create the deviceComplianceActionItem.</span></span>

|<span data-ttu-id="fa73b-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fa73b-128">Property</span></span>|<span data-ttu-id="fa73b-129">種類</span><span class="sxs-lookup"><span data-stu-id="fa73b-129">Type</span></span>|<span data-ttu-id="fa73b-130">説明</span><span class="sxs-lookup"><span data-stu-id="fa73b-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fa73b-131">ID</span><span class="sxs-lookup"><span data-stu-id="fa73b-131">id</span></span>|<span data-ttu-id="fa73b-132">String</span><span class="sxs-lookup"><span data-stu-id="fa73b-132">String</span></span>|<span data-ttu-id="fa73b-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="fa73b-133">Key of the entity.</span></span>|
|<span data-ttu-id="fa73b-134">gracePeriodHours</span><span class="sxs-lookup"><span data-stu-id="fa73b-134">gracePeriodHours</span></span>|<span data-ttu-id="fa73b-135">Int32</span><span class="sxs-lookup"><span data-stu-id="fa73b-135">Int32</span></span>|<span data-ttu-id="fa73b-136">アクションが実行されるまでの待機時間。</span><span class="sxs-lookup"><span data-stu-id="fa73b-136">Number of hours to wait till the action will be enforced.</span></span> <span data-ttu-id="fa73b-137">有効な値は 0 から 8760 までです</span><span class="sxs-lookup"><span data-stu-id="fa73b-137">Valid values 0 to 8760</span></span>|
|<span data-ttu-id="fa73b-138">actionType</span><span class="sxs-lookup"><span data-stu-id="fa73b-138">actionType</span></span>|[<span data-ttu-id="fa73b-139">deviceComplianceActionType</span><span class="sxs-lookup"><span data-stu-id="fa73b-139">deviceComplianceActionType</span></span>](../resources/intune-deviceconfig-devicecomplianceactiontype.md)|<span data-ttu-id="fa73b-140">実行するアクションです。</span><span class="sxs-lookup"><span data-stu-id="fa73b-140">What action to take.</span></span> <span data-ttu-id="fa73b-141">可能な値は、`noAction`、`notification`、`block`、`retire`、`wipe`、`removeResourceAccessProfiles`、`pushNotification` です。</span><span class="sxs-lookup"><span data-stu-id="fa73b-141">Possible values are: `noAction`, `notification`, `block`, `retire`, `wipe`, `removeResourceAccessProfiles`, `pushNotification`.</span></span>|
|<span data-ttu-id="fa73b-142">notificationTemplateId</span><span class="sxs-lookup"><span data-stu-id="fa73b-142">notificationTemplateId</span></span>|<span data-ttu-id="fa73b-143">String</span><span class="sxs-lookup"><span data-stu-id="fa73b-143">String</span></span>|<span data-ttu-id="fa73b-144">使用する通知メッセージ テンプレート</span><span class="sxs-lookup"><span data-stu-id="fa73b-144">What notification Message template to use</span></span>|
|<span data-ttu-id="fa73b-145">notificationMessageCCList</span><span class="sxs-lookup"><span data-stu-id="fa73b-145">notificationMessageCCList</span></span>|<span data-ttu-id="fa73b-146">String コレクション</span><span class="sxs-lookup"><span data-stu-id="fa73b-146">String collection</span></span>|<span data-ttu-id="fa73b-147">この通知メッセージの CC に設定するグループ ID のリスト。</span><span class="sxs-lookup"><span data-stu-id="fa73b-147">A list of group IDs to speicify who to CC this notification message to.</span></span>|



## <a name="response"></a><span data-ttu-id="fa73b-148">応答</span><span class="sxs-lookup"><span data-stu-id="fa73b-148">Response</span></span>
<span data-ttu-id="fa73b-149">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="fa73b-149">If successful, this method returns a `201 Created` response code and a [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fa73b-150">例</span><span class="sxs-lookup"><span data-stu-id="fa73b-150">Example</span></span>
### <a name="request"></a><span data-ttu-id="fa73b-151">要求</span><span class="sxs-lookup"><span data-stu-id="fa73b-151">Request</span></span>
<span data-ttu-id="fa73b-152">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="fa73b-152">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations
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

### <a name="response"></a><span data-ttu-id="fa73b-153">応答</span><span class="sxs-lookup"><span data-stu-id="fa73b-153">Response</span></span>
<span data-ttu-id="fa73b-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="fa73b-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



