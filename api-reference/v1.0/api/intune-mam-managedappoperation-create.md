---
title: managedAppOperation の作成
description: 新しい managedAppOperation オブジェクトを作成します。
ms.openlocfilehash: 083ecd75da542a80ce06213725db9594941504eb
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27023761"
---
# <a name="create-managedappoperation"></a><span data-ttu-id="05862-103">managedAppOperation の作成</span><span class="sxs-lookup"><span data-stu-id="05862-103">Create managedAppOperation</span></span>

> <span data-ttu-id="05862-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="05862-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="05862-105">新しい [managedAppOperation](../resources/intune-mam-managedappoperation.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="05862-105">Create a new [managedAppOperation](../resources/intune-mam-managedappoperation.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="05862-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="05862-106">Prerequisites</span></span>
<span data-ttu-id="05862-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="05862-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="05862-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="05862-109">Permission type</span></span>|<span data-ttu-id="05862-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="05862-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="05862-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="05862-111">Delegated (work or school account)</span></span>|<span data-ttu-id="05862-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="05862-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="05862-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="05862-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="05862-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="05862-114">Not supported.</span></span>|
|<span data-ttu-id="05862-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="05862-115">Application</span></span>|<span data-ttu-id="05862-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="05862-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="05862-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="05862-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/operations
```

## <a name="request-headers"></a><span data-ttu-id="05862-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="05862-118">Request headers</span></span>
|<span data-ttu-id="05862-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="05862-119">Header</span></span>|<span data-ttu-id="05862-120">値</span><span class="sxs-lookup"><span data-stu-id="05862-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="05862-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="05862-121">Authorization</span></span>|<span data-ttu-id="05862-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="05862-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="05862-123">Accept</span><span class="sxs-lookup"><span data-stu-id="05862-123">Accept</span></span>|<span data-ttu-id="05862-124">application/json</span><span class="sxs-lookup"><span data-stu-id="05862-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="05862-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="05862-125">Request body</span></span>
<span data-ttu-id="05862-126">要求本文で、managedAppOperation オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="05862-126">In the request body, supply a JSON representation for the managedAppOperation object.</span></span>

<span data-ttu-id="05862-127">次の表に、managedAppOperation の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="05862-127">The following table shows the properties that are required when you create the managedAppOperation.</span></span>

|<span data-ttu-id="05862-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="05862-128">Property</span></span>|<span data-ttu-id="05862-129">型</span><span class="sxs-lookup"><span data-stu-id="05862-129">Type</span></span>|<span data-ttu-id="05862-130">説明</span><span class="sxs-lookup"><span data-stu-id="05862-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="05862-131">displayName</span><span class="sxs-lookup"><span data-stu-id="05862-131">displayName</span></span>|<span data-ttu-id="05862-132">String</span><span class="sxs-lookup"><span data-stu-id="05862-132">String</span></span>|<span data-ttu-id="05862-133">操作名。</span><span class="sxs-lookup"><span data-stu-id="05862-133">The operation name.</span></span>|
|<span data-ttu-id="05862-134">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="05862-134">lastModifiedDateTime</span></span>|<span data-ttu-id="05862-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="05862-135">DateTimeOffset</span></span>|<span data-ttu-id="05862-136">アプリ操作が変更された最終時刻。</span><span class="sxs-lookup"><span data-stu-id="05862-136">The last time the app operation was modified.</span></span>|
|<span data-ttu-id="05862-137">state</span><span class="sxs-lookup"><span data-stu-id="05862-137">state</span></span>|<span data-ttu-id="05862-138">String</span><span class="sxs-lookup"><span data-stu-id="05862-138">String</span></span>|<span data-ttu-id="05862-139">操作の現在の状態。</span><span class="sxs-lookup"><span data-stu-id="05862-139">The current state of the operation</span></span>|
|<span data-ttu-id="05862-140">id</span><span class="sxs-lookup"><span data-stu-id="05862-140">id</span></span>|<span data-ttu-id="05862-141">String</span><span class="sxs-lookup"><span data-stu-id="05862-141">String</span></span>|<span data-ttu-id="05862-142">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="05862-142">Key of the entity.</span></span>|
|<span data-ttu-id="05862-143">version</span><span class="sxs-lookup"><span data-stu-id="05862-143">version</span></span>|<span data-ttu-id="05862-144">String</span><span class="sxs-lookup"><span data-stu-id="05862-144">String</span></span>|<span data-ttu-id="05862-145">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="05862-145">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="05862-146">応答</span><span class="sxs-lookup"><span data-stu-id="05862-146">Response</span></span>
<span data-ttu-id="05862-147">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [managedAppOperation](../resources/intune-mam-managedappoperation.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="05862-147">If successful, this method returns a `201 Created` response code and a [managedAppOperation](../resources/intune-mam-managedappoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="05862-148">例</span><span class="sxs-lookup"><span data-stu-id="05862-148">Example</span></span>
### <a name="request"></a><span data-ttu-id="05862-149">要求</span><span class="sxs-lookup"><span data-stu-id="05862-149">Request</span></span>
<span data-ttu-id="05862-150">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="05862-150">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/operations
Content-type: application/json
Content-length: 159

{
  "@odata.type": "#microsoft.graph.managedAppOperation",
  "displayName": "Display Name value",
  "state": "State value",
  "version": "Version value"
}
```

### <a name="response"></a><span data-ttu-id="05862-151">応答</span><span class="sxs-lookup"><span data-stu-id="05862-151">Response</span></span>
<span data-ttu-id="05862-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="05862-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 272

{
  "@odata.type": "#microsoft.graph.managedAppOperation",
  "displayName": "Display Name value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "state": "State value",
  "id": "f2867b06-7b06-f286-067b-86f2067b86f2",
  "version": "Version value"
}
```


