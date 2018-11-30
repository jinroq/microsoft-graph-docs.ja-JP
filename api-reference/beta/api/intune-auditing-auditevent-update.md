---
title: auditEvent の更新
description: auditEvent オブジェクトのプロパティを更新します。
ms.openlocfilehash: 1a1de92517b59d168147feafe16fe2479b8afc2b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27072858"
---
# <a name="update-auditevent"></a><span data-ttu-id="3bab1-103">auditEvent の更新</span><span class="sxs-lookup"><span data-stu-id="3bab1-103">Update auditEvent</span></span>

> <span data-ttu-id="3bab1-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="3bab1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3bab1-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3bab1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3bab1-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="3bab1-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3bab1-107">[auditEvent](../resources/intune-auditing-auditevent.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="3bab1-107">Update the properties of a [auditEvent](../resources/intune-auditing-auditevent.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3bab1-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="3bab1-108">Prerequisites</span></span>
<span data-ttu-id="3bab1-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3bab1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3bab1-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3bab1-111">Permission type</span></span>|<span data-ttu-id="3bab1-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="3bab1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3bab1-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3bab1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3bab1-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3bab1-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="3bab1-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3bab1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3bab1-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3bab1-116">Not supported.</span></span>|
|<span data-ttu-id="3bab1-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3bab1-117">Application</span></span>|<span data-ttu-id="3bab1-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3bab1-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3bab1-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3bab1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/auditEvents/{auditEventId}
```

## <a name="request-headers"></a><span data-ttu-id="3bab1-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3bab1-120">Request headers</span></span>
|<span data-ttu-id="3bab1-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3bab1-121">Header</span></span>|<span data-ttu-id="3bab1-122">値</span><span class="sxs-lookup"><span data-stu-id="3bab1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3bab1-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3bab1-123">Authorization</span></span>|<span data-ttu-id="3bab1-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="3bab1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3bab1-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3bab1-125">Accept</span></span>|<span data-ttu-id="3bab1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3bab1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3bab1-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="3bab1-127">Request body</span></span>
<span data-ttu-id="3bab1-128">要求本文で、[auditEvent](../resources/intune-auditing-auditevent.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="3bab1-128">In the request body, supply a JSON representation for the [auditEvent](../resources/intune-auditing-auditevent.md) object.</span></span>

<span data-ttu-id="3bab1-129">次の表に、[auditEvent](../resources/intune-auditing-auditevent.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="3bab1-129">The following table shows the properties that are required when you create the [auditEvent](../resources/intune-auditing-auditevent.md).</span></span>

|<span data-ttu-id="3bab1-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3bab1-130">Property</span></span>|<span data-ttu-id="3bab1-131">型</span><span class="sxs-lookup"><span data-stu-id="3bab1-131">Type</span></span>|<span data-ttu-id="3bab1-132">説明</span><span class="sxs-lookup"><span data-stu-id="3bab1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3bab1-133">id</span><span class="sxs-lookup"><span data-stu-id="3bab1-133">id</span></span>|<span data-ttu-id="3bab1-134">String</span><span class="sxs-lookup"><span data-stu-id="3bab1-134">String</span></span>|<span data-ttu-id="3bab1-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="3bab1-135">Key of the entity.</span></span>|
|<span data-ttu-id="3bab1-136">displayName</span><span class="sxs-lookup"><span data-stu-id="3bab1-136">displayName</span></span>|<span data-ttu-id="3bab1-137">String</span><span class="sxs-lookup"><span data-stu-id="3bab1-137">String</span></span>|<span data-ttu-id="3bab1-138">イベントの表示名。</span><span class="sxs-lookup"><span data-stu-id="3bab1-138">Event display name.</span></span>|
|<span data-ttu-id="3bab1-139">componentName</span><span class="sxs-lookup"><span data-stu-id="3bab1-139">componentName</span></span>|<span data-ttu-id="3bab1-140">String</span><span class="sxs-lookup"><span data-stu-id="3bab1-140">String</span></span>|<span data-ttu-id="3bab1-141">コンポーネント名。</span><span class="sxs-lookup"><span data-stu-id="3bab1-141">Component name.</span></span>|
|<span data-ttu-id="3bab1-142">actor</span><span class="sxs-lookup"><span data-stu-id="3bab1-142">actor</span></span>|[<span data-ttu-id="3bab1-143">auditActor</span><span class="sxs-lookup"><span data-stu-id="3bab1-143">auditActor</span></span>](../resources/intune-auditing-auditactor.md)|<span data-ttu-id="3bab1-144">監査イベントに関連付けられている AAD ユーザーとアプリケーション。</span><span class="sxs-lookup"><span data-stu-id="3bab1-144">AAD user and application that are associated with the audit event.</span></span>|
|<span data-ttu-id="3bab1-145">activity</span><span class="sxs-lookup"><span data-stu-id="3bab1-145">activity</span></span>|<span data-ttu-id="3bab1-146">String</span><span class="sxs-lookup"><span data-stu-id="3bab1-146">String</span></span>|<span data-ttu-id="3bab1-147">わかりやすいアクティビティの名前。</span><span class="sxs-lookup"><span data-stu-id="3bab1-147">Friendly name of the activity.</span></span>|
|<span data-ttu-id="3bab1-148">activityDateTime</span><span class="sxs-lookup"><span data-stu-id="3bab1-148">activityDateTime</span></span>|<span data-ttu-id="3bab1-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3bab1-149">DateTimeOffset</span></span>|<span data-ttu-id="3bab1-150">アクティビティが実行された日時 (UTC)。</span><span class="sxs-lookup"><span data-stu-id="3bab1-150">The date time in UTC when the activity was performed.</span></span>|
|<span data-ttu-id="3bab1-151">activityType</span><span class="sxs-lookup"><span data-stu-id="3bab1-151">activityType</span></span>|<span data-ttu-id="3bab1-152">String</span><span class="sxs-lookup"><span data-stu-id="3bab1-152">String</span></span>|<span data-ttu-id="3bab1-153">実行されたアクティビティの種類。</span><span class="sxs-lookup"><span data-stu-id="3bab1-153">The type of activity that was being performed.</span></span>|
|<span data-ttu-id="3bab1-154">activityOperationType</span><span class="sxs-lookup"><span data-stu-id="3bab1-154">activityOperationType</span></span>|<span data-ttu-id="3bab1-155">String</span><span class="sxs-lookup"><span data-stu-id="3bab1-155">String</span></span>|<span data-ttu-id="3bab1-156">アクティビティの HTTP 操作の種類。</span><span class="sxs-lookup"><span data-stu-id="3bab1-156">The HTTP operation type of the activity.</span></span>|
|<span data-ttu-id="3bab1-157">activityResult</span><span class="sxs-lookup"><span data-stu-id="3bab1-157">activityResult</span></span>|<span data-ttu-id="3bab1-158">String</span><span class="sxs-lookup"><span data-stu-id="3bab1-158">String</span></span>|<span data-ttu-id="3bab1-159">アクティビティの結果。</span><span class="sxs-lookup"><span data-stu-id="3bab1-159">The result of the activity.</span></span>|
|<span data-ttu-id="3bab1-160">correlationId</span><span class="sxs-lookup"><span data-stu-id="3bab1-160">correlationId</span></span>|<span data-ttu-id="3bab1-161">Guid</span><span class="sxs-lookup"><span data-stu-id="3bab1-161">Guid</span></span>|<span data-ttu-id="3bab1-162">システム内でのアクティビティに関連付けるために使用されるクライアント要求 ID。</span><span class="sxs-lookup"><span data-stu-id="3bab1-162">The client request Id that is used to correlate activity within the system.</span></span>|
|<span data-ttu-id="3bab1-163">resources</span><span class="sxs-lookup"><span data-stu-id="3bab1-163">resources</span></span>|<span data-ttu-id="3bab1-164">[auditResource](../resources/intune-auditing-auditresource.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="3bab1-164">[auditResource](../resources/intune-auditing-auditresource.md) collection</span></span>|<span data-ttu-id="3bab1-165">変更中のリソースです。</span><span class="sxs-lookup"><span data-stu-id="3bab1-165">Resources being modified.</span></span>|
|<span data-ttu-id="3bab1-166">category</span><span class="sxs-lookup"><span data-stu-id="3bab1-166">category</span></span>|<span data-ttu-id="3bab1-167">String</span><span class="sxs-lookup"><span data-stu-id="3bab1-167">String</span></span>|<span data-ttu-id="3bab1-168">監査のカテゴリです。</span><span class="sxs-lookup"><span data-stu-id="3bab1-168">Audit category.</span></span>|



## <a name="response"></a><span data-ttu-id="3bab1-169">応答</span><span class="sxs-lookup"><span data-stu-id="3bab1-169">Response</span></span>
<span data-ttu-id="3bab1-170">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [auditEvent](../resources/intune-auditing-auditevent.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="3bab1-170">If successful, this method returns a `200 OK` response code and an updated [auditEvent](../resources/intune-auditing-auditevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3bab1-171">例</span><span class="sxs-lookup"><span data-stu-id="3bab1-171">Example</span></span>
### <a name="request"></a><span data-ttu-id="3bab1-172">要求</span><span class="sxs-lookup"><span data-stu-id="3bab1-172">Request</span></span>
<span data-ttu-id="3bab1-173">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="3bab1-173">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/auditEvents/{auditEventId}
Content-type: application/json
Content-length: 1341

{
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

### <a name="response"></a><span data-ttu-id="3bab1-174">応答</span><span class="sxs-lookup"><span data-stu-id="3bab1-174">Response</span></span>
<span data-ttu-id="3bab1-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="3bab1-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





