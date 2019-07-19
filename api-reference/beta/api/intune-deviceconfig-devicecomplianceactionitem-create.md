---
title: deviceComplianceActionItem の作成
description: 新しい deviceComplianceActionItem オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9807dc7dbb09d64ae0af3770155812747cc37cec
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34968645"
---
# <a name="create-devicecomplianceactionitem"></a><span data-ttu-id="7e639-103">deviceComplianceActionItem の作成</span><span class="sxs-lookup"><span data-stu-id="7e639-103">Create deviceComplianceActionItem</span></span>

> <span data-ttu-id="7e639-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7e639-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7e639-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="7e639-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7e639-106">新しい [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="7e639-106">Create a new [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7e639-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="7e639-107">Prerequisites</span></span>
<span data-ttu-id="7e639-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7e639-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7e639-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7e639-110">Permission type</span></span>|<span data-ttu-id="7e639-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="7e639-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7e639-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7e639-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7e639-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7e639-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7e639-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7e639-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7e639-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7e639-115">Not supported.</span></span>|
|<span data-ttu-id="7e639-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7e639-116">Application</span></span>|<span data-ttu-id="7e639-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7e639-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7e639-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7e639-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="7e639-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7e639-119">Request headers</span></span>
|<span data-ttu-id="7e639-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7e639-120">Header</span></span>|<span data-ttu-id="7e639-121">値</span><span class="sxs-lookup"><span data-stu-id="7e639-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7e639-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="7e639-122">Authorization</span></span>|<span data-ttu-id="7e639-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="7e639-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7e639-124">承諾</span><span class="sxs-lookup"><span data-stu-id="7e639-124">Accept</span></span>|<span data-ttu-id="7e639-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7e639-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7e639-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="7e639-126">Request body</span></span>
<span data-ttu-id="7e639-127">要求本文で、deviceComplianceActionItem オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="7e639-127">In the request body, supply a JSON representation for the deviceComplianceActionItem object.</span></span>

<span data-ttu-id="7e639-128">次の表に、deviceComplianceActionItem の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="7e639-128">The following table shows the properties that are required when you create the deviceComplianceActionItem.</span></span>

|<span data-ttu-id="7e639-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7e639-129">Property</span></span>|<span data-ttu-id="7e639-130">型</span><span class="sxs-lookup"><span data-stu-id="7e639-130">Type</span></span>|<span data-ttu-id="7e639-131">説明</span><span class="sxs-lookup"><span data-stu-id="7e639-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7e639-132">id</span><span class="sxs-lookup"><span data-stu-id="7e639-132">id</span></span>|<span data-ttu-id="7e639-133">String</span><span class="sxs-lookup"><span data-stu-id="7e639-133">String</span></span>|<span data-ttu-id="7e639-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="7e639-134">Key of the entity.</span></span>|
|<span data-ttu-id="7e639-135">gracePeriodHours</span><span class="sxs-lookup"><span data-stu-id="7e639-135">gracePeriodHours</span></span>|<span data-ttu-id="7e639-136">Int32</span><span class="sxs-lookup"><span data-stu-id="7e639-136">Int32</span></span>|<span data-ttu-id="7e639-137">アクションが実行されるまでの待機時間。</span><span class="sxs-lookup"><span data-stu-id="7e639-137">Number of hours to wait till the action will be enforced.</span></span> <span data-ttu-id="7e639-138">有効な値は 0 から 8760 までです</span><span class="sxs-lookup"><span data-stu-id="7e639-138">Valid values 0 to 8760</span></span>|
|<span data-ttu-id="7e639-139">actionType</span><span class="sxs-lookup"><span data-stu-id="7e639-139">actionType</span></span>|[<span data-ttu-id="7e639-140">deviceComplianceActionType</span><span class="sxs-lookup"><span data-stu-id="7e639-140">deviceComplianceActionType</span></span>](../resources/intune-deviceconfig-devicecomplianceactiontype.md)|<span data-ttu-id="7e639-141">実行するアクション。</span><span class="sxs-lookup"><span data-stu-id="7e639-141">What action to take.</span></span> <span data-ttu-id="7e639-142">可能な値は、`noAction`、`notification`、`block`、`retire`、`wipe`、`removeResourceAccessProfiles`、`pushNotification`、`remoteLock` です。</span><span class="sxs-lookup"><span data-stu-id="7e639-142">Possible values are: `noAction`, `notification`, `block`, `retire`, `wipe`, `removeResourceAccessProfiles`, `pushNotification`, `remoteLock`.</span></span>|
|<span data-ttu-id="7e639-143">notificationTemplateId</span><span class="sxs-lookup"><span data-stu-id="7e639-143">notificationTemplateId</span></span>|<span data-ttu-id="7e639-144">String</span><span class="sxs-lookup"><span data-stu-id="7e639-144">String</span></span>|<span data-ttu-id="7e639-145">使用する通知メッセージ テンプレート</span><span class="sxs-lookup"><span data-stu-id="7e639-145">What notification Message template to use</span></span>|
|<span data-ttu-id="7e639-146">notificationMessageCCList</span><span class="sxs-lookup"><span data-stu-id="7e639-146">notificationMessageCCList</span></span>|<span data-ttu-id="7e639-147">String コレクション</span><span class="sxs-lookup"><span data-stu-id="7e639-147">String collection</span></span>|<span data-ttu-id="7e639-148">この通知メッセージの CC に設定するグループ ID のリスト。</span><span class="sxs-lookup"><span data-stu-id="7e639-148">A list of group IDs to speicify who to CC this notification message to.</span></span>|



## <a name="response"></a><span data-ttu-id="7e639-149">応答</span><span class="sxs-lookup"><span data-stu-id="7e639-149">Response</span></span>
<span data-ttu-id="7e639-150">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="7e639-150">If successful, this method returns a `201 Created` response code and a [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7e639-151">例</span><span class="sxs-lookup"><span data-stu-id="7e639-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="7e639-152">要求</span><span class="sxs-lookup"><span data-stu-id="7e639-152">Request</span></span>
<span data-ttu-id="7e639-153">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="7e639-153">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="7e639-154">応答</span><span class="sxs-lookup"><span data-stu-id="7e639-154">Response</span></span>
<span data-ttu-id="7e639-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="7e639-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





