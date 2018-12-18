---
title: deviceComplianceActionItem の作成
description: 新しい deviceComplianceActionItem オブジェクトを作成します。
author: tfitzmac
ms.openlocfilehash: 52dd6bca4aa4f91f68d6e986a69e061e899602e8
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27356120"
---
# <a name="create-devicecomplianceactionitem"></a><span data-ttu-id="0254c-103">deviceComplianceActionItem の作成</span><span class="sxs-lookup"><span data-stu-id="0254c-103">Create deviceComplianceActionItem</span></span>

> <span data-ttu-id="0254c-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="0254c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0254c-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0254c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0254c-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="0254c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0254c-107">新しい [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="0254c-107">Create a new [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0254c-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="0254c-108">Prerequisites</span></span>
<span data-ttu-id="0254c-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0254c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0254c-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0254c-111">Permission type</span></span>|<span data-ttu-id="0254c-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="0254c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0254c-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0254c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0254c-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0254c-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0254c-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0254c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0254c-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0254c-116">Not supported.</span></span>|
|<span data-ttu-id="0254c-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0254c-117">Application</span></span>|<span data-ttu-id="0254c-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0254c-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0254c-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0254c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="0254c-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0254c-120">Request headers</span></span>
|<span data-ttu-id="0254c-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0254c-121">Header</span></span>|<span data-ttu-id="0254c-122">値</span><span class="sxs-lookup"><span data-stu-id="0254c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0254c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0254c-123">Authorization</span></span>|<span data-ttu-id="0254c-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="0254c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0254c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0254c-125">Accept</span></span>|<span data-ttu-id="0254c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0254c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0254c-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="0254c-127">Request body</span></span>
<span data-ttu-id="0254c-128">要求本文で、deviceComplianceActionItem オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="0254c-128">In the request body, supply a JSON representation for the deviceComplianceActionItem object.</span></span>

<span data-ttu-id="0254c-129">次の表に、deviceComplianceActionItem の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="0254c-129">The following table shows the properties that are required when you create the deviceComplianceActionItem.</span></span>

|<span data-ttu-id="0254c-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0254c-130">Property</span></span>|<span data-ttu-id="0254c-131">種類</span><span class="sxs-lookup"><span data-stu-id="0254c-131">Type</span></span>|<span data-ttu-id="0254c-132">説明</span><span class="sxs-lookup"><span data-stu-id="0254c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0254c-133">ID</span><span class="sxs-lookup"><span data-stu-id="0254c-133">id</span></span>|<span data-ttu-id="0254c-134">String</span><span class="sxs-lookup"><span data-stu-id="0254c-134">String</span></span>|<span data-ttu-id="0254c-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="0254c-135">Key of the entity.</span></span>|
|<span data-ttu-id="0254c-136">gracePeriodHours</span><span class="sxs-lookup"><span data-stu-id="0254c-136">gracePeriodHours</span></span>|<span data-ttu-id="0254c-137">Int32</span><span class="sxs-lookup"><span data-stu-id="0254c-137">Int32</span></span>|<span data-ttu-id="0254c-138">アクションが実行されるまでの待機時間。</span><span class="sxs-lookup"><span data-stu-id="0254c-138">Number of hours to wait till the action will be enforced.</span></span> <span data-ttu-id="0254c-139">有効な値は 0 から 8760 までです</span><span class="sxs-lookup"><span data-stu-id="0254c-139">Valid values 0 to 8760</span></span>|
|<span data-ttu-id="0254c-140">actionType</span><span class="sxs-lookup"><span data-stu-id="0254c-140">actionType</span></span>|[<span data-ttu-id="0254c-141">deviceComplianceActionType</span><span class="sxs-lookup"><span data-stu-id="0254c-141">deviceComplianceActionType</span></span>](../resources/intune-deviceconfig-devicecomplianceactiontype.md)|<span data-ttu-id="0254c-142">実行するアクションです。</span><span class="sxs-lookup"><span data-stu-id="0254c-142">What action to take.</span></span> <span data-ttu-id="0254c-143">可能な値は、`noAction`、`notification`、`block`、`retire`、`wipe`、`removeResourceAccessProfiles`、`pushNotification`、`remoteLock` です。</span><span class="sxs-lookup"><span data-stu-id="0254c-143">Possible values are: `noAction`, `notification`, `block`, `retire`, `wipe`, `removeResourceAccessProfiles`, `pushNotification`, `remoteLock`.</span></span>|
|<span data-ttu-id="0254c-144">notificationTemplateId</span><span class="sxs-lookup"><span data-stu-id="0254c-144">notificationTemplateId</span></span>|<span data-ttu-id="0254c-145">String</span><span class="sxs-lookup"><span data-stu-id="0254c-145">String</span></span>|<span data-ttu-id="0254c-146">使用する通知メッセージ テンプレート</span><span class="sxs-lookup"><span data-stu-id="0254c-146">What notification Message template to use</span></span>|
|<span data-ttu-id="0254c-147">notificationMessageCCList</span><span class="sxs-lookup"><span data-stu-id="0254c-147">notificationMessageCCList</span></span>|<span data-ttu-id="0254c-148">String コレクション</span><span class="sxs-lookup"><span data-stu-id="0254c-148">String collection</span></span>|<span data-ttu-id="0254c-149">この通知メッセージの CC に設定するグループ ID のリスト。</span><span class="sxs-lookup"><span data-stu-id="0254c-149">A list of group IDs to speicify who to CC this notification message to.</span></span>|



## <a name="response"></a><span data-ttu-id="0254c-150">応答</span><span class="sxs-lookup"><span data-stu-id="0254c-150">Response</span></span>
<span data-ttu-id="0254c-151">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="0254c-151">If successful, this method returns a `201 Created` response code and a [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0254c-152">例</span><span class="sxs-lookup"><span data-stu-id="0254c-152">Example</span></span>
### <a name="request"></a><span data-ttu-id="0254c-153">要求</span><span class="sxs-lookup"><span data-stu-id="0254c-153">Request</span></span>
<span data-ttu-id="0254c-154">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="0254c-154">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations
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

### <a name="response"></a><span data-ttu-id="0254c-155">応答</span><span class="sxs-lookup"><span data-stu-id="0254c-155">Response</span></span>
<span data-ttu-id="0254c-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="0254c-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





