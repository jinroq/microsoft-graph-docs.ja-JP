---
title: auditEvent の作成
description: 新しい auditEvent オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: b6b673e2c7090ecfee3368d76f4690dd309ffdd0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27980280"
---
# <a name="create-auditevent"></a><span data-ttu-id="a5980-103">auditEvent の作成</span><span class="sxs-lookup"><span data-stu-id="a5980-103">Create auditEvent</span></span>

> <span data-ttu-id="a5980-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="a5980-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a5980-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a5980-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a5980-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="a5980-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a5980-107">新しい [auditEvent](../resources/intune-auditing-auditevent.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="a5980-107">Create a new [auditEvent](../resources/intune-auditing-auditevent.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a5980-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="a5980-108">Prerequisites</span></span>
<span data-ttu-id="a5980-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a5980-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a5980-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a5980-111">Permission type</span></span>|<span data-ttu-id="a5980-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="a5980-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a5980-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a5980-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a5980-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a5980-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="a5980-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a5980-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a5980-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a5980-116">Not supported.</span></span>|
|<span data-ttu-id="a5980-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a5980-117">Application</span></span>|<span data-ttu-id="a5980-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a5980-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a5980-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a5980-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/auditEvents
```

## <a name="request-headers"></a><span data-ttu-id="a5980-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a5980-120">Request headers</span></span>
|<span data-ttu-id="a5980-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a5980-121">Header</span></span>|<span data-ttu-id="a5980-122">値</span><span class="sxs-lookup"><span data-stu-id="a5980-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a5980-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a5980-123">Authorization</span></span>|<span data-ttu-id="a5980-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="a5980-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a5980-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a5980-125">Accept</span></span>|<span data-ttu-id="a5980-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a5980-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a5980-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="a5980-127">Request body</span></span>
<span data-ttu-id="a5980-128">要求本文で、auditEvent オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="a5980-128">In the request body, supply a JSON representation for the auditEvent object.</span></span>

<span data-ttu-id="a5980-129">次の表に、auditEvent の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="a5980-129">The following table shows the properties that are required when you create the auditEvent.</span></span>

|<span data-ttu-id="a5980-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a5980-130">Property</span></span>|<span data-ttu-id="a5980-131">型</span><span class="sxs-lookup"><span data-stu-id="a5980-131">Type</span></span>|<span data-ttu-id="a5980-132">説明</span><span class="sxs-lookup"><span data-stu-id="a5980-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a5980-133">ID</span><span class="sxs-lookup"><span data-stu-id="a5980-133">id</span></span>|<span data-ttu-id="a5980-134">String</span><span class="sxs-lookup"><span data-stu-id="a5980-134">String</span></span>|<span data-ttu-id="a5980-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="a5980-135">Key of the entity.</span></span>|
|<span data-ttu-id="a5980-136">displayName</span><span class="sxs-lookup"><span data-stu-id="a5980-136">displayName</span></span>|<span data-ttu-id="a5980-137">String</span><span class="sxs-lookup"><span data-stu-id="a5980-137">String</span></span>|<span data-ttu-id="a5980-138">イベントの表示名。</span><span class="sxs-lookup"><span data-stu-id="a5980-138">Event display name.</span></span>|
|<span data-ttu-id="a5980-139">componentName</span><span class="sxs-lookup"><span data-stu-id="a5980-139">componentName</span></span>|<span data-ttu-id="a5980-140">String</span><span class="sxs-lookup"><span data-stu-id="a5980-140">String</span></span>|<span data-ttu-id="a5980-141">コンポーネント名。</span><span class="sxs-lookup"><span data-stu-id="a5980-141">Component name.</span></span>|
|<span data-ttu-id="a5980-142">actor</span><span class="sxs-lookup"><span data-stu-id="a5980-142">actor</span></span>|[<span data-ttu-id="a5980-143">auditActor</span><span class="sxs-lookup"><span data-stu-id="a5980-143">auditActor</span></span>](../resources/intune-auditing-auditactor.md)|<span data-ttu-id="a5980-144">監査イベントに関連付けられている AAD ユーザーとアプリケーション。</span><span class="sxs-lookup"><span data-stu-id="a5980-144">AAD user and application that are associated with the audit event.</span></span>|
|<span data-ttu-id="a5980-145">activity</span><span class="sxs-lookup"><span data-stu-id="a5980-145">activity</span></span>|<span data-ttu-id="a5980-146">String</span><span class="sxs-lookup"><span data-stu-id="a5980-146">String</span></span>|<span data-ttu-id="a5980-147">わかりやすいアクティビティの名前。</span><span class="sxs-lookup"><span data-stu-id="a5980-147">Friendly name of the activity.</span></span>|
|<span data-ttu-id="a5980-148">activityDateTime</span><span class="sxs-lookup"><span data-stu-id="a5980-148">activityDateTime</span></span>|<span data-ttu-id="a5980-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a5980-149">DateTimeOffset</span></span>|<span data-ttu-id="a5980-150">アクティビティが実行された日時 (UTC)。</span><span class="sxs-lookup"><span data-stu-id="a5980-150">The date time in UTC when the activity was performed.</span></span>|
|<span data-ttu-id="a5980-151">activityType</span><span class="sxs-lookup"><span data-stu-id="a5980-151">activityType</span></span>|<span data-ttu-id="a5980-152">String</span><span class="sxs-lookup"><span data-stu-id="a5980-152">String</span></span>|<span data-ttu-id="a5980-153">実行されたアクティビティの種類。</span><span class="sxs-lookup"><span data-stu-id="a5980-153">The type of activity that was being performed.</span></span>|
|<span data-ttu-id="a5980-154">activityOperationType</span><span class="sxs-lookup"><span data-stu-id="a5980-154">activityOperationType</span></span>|<span data-ttu-id="a5980-155">String</span><span class="sxs-lookup"><span data-stu-id="a5980-155">String</span></span>|<span data-ttu-id="a5980-156">アクティビティの HTTP 操作の種類。</span><span class="sxs-lookup"><span data-stu-id="a5980-156">The HTTP operation type of the activity.</span></span>|
|<span data-ttu-id="a5980-157">activityResult</span><span class="sxs-lookup"><span data-stu-id="a5980-157">activityResult</span></span>|<span data-ttu-id="a5980-158">String</span><span class="sxs-lookup"><span data-stu-id="a5980-158">String</span></span>|<span data-ttu-id="a5980-159">アクティビティの結果。</span><span class="sxs-lookup"><span data-stu-id="a5980-159">The result of the activity.</span></span>|
|<span data-ttu-id="a5980-160">correlationId</span><span class="sxs-lookup"><span data-stu-id="a5980-160">correlationId</span></span>|<span data-ttu-id="a5980-161">Guid</span><span class="sxs-lookup"><span data-stu-id="a5980-161">Guid</span></span>|<span data-ttu-id="a5980-162">システム内でのアクティビティに関連付けるために使用されるクライアント要求 ID。</span><span class="sxs-lookup"><span data-stu-id="a5980-162">The client request Id that is used to correlate activity within the system.</span></span>|
|<span data-ttu-id="a5980-163">resources</span><span class="sxs-lookup"><span data-stu-id="a5980-163">resources</span></span>|<span data-ttu-id="a5980-164">[auditResource](../resources/intune-auditing-auditresource.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="a5980-164">[auditResource](../resources/intune-auditing-auditresource.md) collection</span></span>|<span data-ttu-id="a5980-165">変更中のリソースです。</span><span class="sxs-lookup"><span data-stu-id="a5980-165">Resources being modified.</span></span>|
|<span data-ttu-id="a5980-166">category</span><span class="sxs-lookup"><span data-stu-id="a5980-166">category</span></span>|<span data-ttu-id="a5980-167">String</span><span class="sxs-lookup"><span data-stu-id="a5980-167">String</span></span>|<span data-ttu-id="a5980-168">監査のカテゴリです。</span><span class="sxs-lookup"><span data-stu-id="a5980-168">Audit category.</span></span>|



## <a name="response"></a><span data-ttu-id="a5980-169">応答</span><span class="sxs-lookup"><span data-stu-id="a5980-169">Response</span></span>
<span data-ttu-id="a5980-170">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [auditEvent](../resources/intune-auditing-auditevent.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="a5980-170">If successful, this method returns a `201 Created` response code and a [auditEvent](../resources/intune-auditing-auditevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a5980-171">例</span><span class="sxs-lookup"><span data-stu-id="a5980-171">Example</span></span>
### <a name="request"></a><span data-ttu-id="a5980-172">要求</span><span class="sxs-lookup"><span data-stu-id="a5980-172">Request</span></span>
<span data-ttu-id="a5980-173">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="a5980-173">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/auditEvents
Content-type: application/json
Content-length: 1390

{
  "@odata.type": "#microsoft.graph.auditEvent",
  "displayName": "Display Name value",
  "componentName": "Component Name value",
  "actor": {
    "@odata.type": "microsoft.graph.auditActor",
    "type": "Type value",
    "userPermissions": [
      "User Permissions value"
    ],
    "applicationId": "Application Id value",
    "applicationDisplayName": "Application Display Name value",
    "userPrincipalName": "User Principal Name value",
    "servicePrincipalName": "Service Principal Name value",
    "ipAddress": "Ip Address value",
    "userId": "User Id value"
  },
  "activity": "Activity value",
  "activityDateTime": "2016-12-31T23:59:51.6363086-08:00",
  "activityType": "Activity Type value",
  "activityOperationType": "Activity Operation Type value",
  "activityResult": "Activity Result value",
  "correlationId": "52effe71-fe71-52ef-71fe-ef5271feef52",
  "resources": [
    {
      "@odata.type": "microsoft.graph.auditResource",
      "displayName": "Display Name value",
      "modifiedProperties": [
        {
          "@odata.type": "microsoft.graph.auditProperty",
          "displayName": "Display Name value",
          "oldValue": "Old Value value",
          "newValue": "New Value value"
        }
      ],
      "type": "Type value",
      "resourceId": "Resource Id value"
    }
  ],
  "category": "Category value"
}
```

### <a name="response"></a><span data-ttu-id="a5980-174">応答</span><span class="sxs-lookup"><span data-stu-id="a5980-174">Response</span></span>
<span data-ttu-id="a5980-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="a5980-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1439

{
  "@odata.type": "#microsoft.graph.auditEvent",
  "id": "59653ce8-3ce8-5965-e83c-6559e83c6559",
  "displayName": "Display Name value",
  "componentName": "Component Name value",
  "actor": {
    "@odata.type": "microsoft.graph.auditActor",
    "type": "Type value",
    "userPermissions": [
      "User Permissions value"
    ],
    "applicationId": "Application Id value",
    "applicationDisplayName": "Application Display Name value",
    "userPrincipalName": "User Principal Name value",
    "servicePrincipalName": "Service Principal Name value",
    "ipAddress": "Ip Address value",
    "userId": "User Id value"
  },
  "activity": "Activity value",
  "activityDateTime": "2016-12-31T23:59:51.6363086-08:00",
  "activityType": "Activity Type value",
  "activityOperationType": "Activity Operation Type value",
  "activityResult": "Activity Result value",
  "correlationId": "52effe71-fe71-52ef-71fe-ef5271feef52",
  "resources": [
    {
      "@odata.type": "microsoft.graph.auditResource",
      "displayName": "Display Name value",
      "modifiedProperties": [
        {
          "@odata.type": "microsoft.graph.auditProperty",
          "displayName": "Display Name value",
          "oldValue": "Old Value value",
          "newValue": "New Value value"
        }
      ],
      "type": "Type value",
      "resourceId": "Resource Id value"
    }
  ],
  "category": "Category value"
}
```





