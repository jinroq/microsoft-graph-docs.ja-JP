---
title: managedAppOperation の作成
description: 新しい managedAppOperation オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: c4afd179a33202eb7780495228f94f23326c7268
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27855210"
---
# <a name="create-managedappoperation"></a><span data-ttu-id="baf26-103">managedAppOperation の作成</span><span class="sxs-lookup"><span data-stu-id="baf26-103">Create managedAppOperation</span></span>

> <span data-ttu-id="baf26-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="baf26-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="baf26-105">新しい [managedAppOperation](../resources/intune-mam-managedappoperation.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="baf26-105">Create a new [managedAppOperation](../resources/intune-mam-managedappoperation.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="baf26-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="baf26-106">Prerequisites</span></span>
<span data-ttu-id="baf26-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="baf26-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="baf26-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="baf26-109">Permission type</span></span>|<span data-ttu-id="baf26-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="baf26-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="baf26-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="baf26-111">Delegated (work or school account)</span></span>|<span data-ttu-id="baf26-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="baf26-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="baf26-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="baf26-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="baf26-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="baf26-114">Not supported.</span></span>|
|<span data-ttu-id="baf26-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="baf26-115">Application</span></span>|<span data-ttu-id="baf26-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="baf26-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="baf26-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="baf26-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/operations
```

## <a name="request-headers"></a><span data-ttu-id="baf26-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="baf26-118">Request headers</span></span>
|<span data-ttu-id="baf26-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="baf26-119">Header</span></span>|<span data-ttu-id="baf26-120">値</span><span class="sxs-lookup"><span data-stu-id="baf26-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="baf26-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="baf26-121">Authorization</span></span>|<span data-ttu-id="baf26-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="baf26-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="baf26-123">Accept</span><span class="sxs-lookup"><span data-stu-id="baf26-123">Accept</span></span>|<span data-ttu-id="baf26-124">application/json</span><span class="sxs-lookup"><span data-stu-id="baf26-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="baf26-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="baf26-125">Request body</span></span>
<span data-ttu-id="baf26-126">要求本文で、managedAppOperation オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="baf26-126">In the request body, supply a JSON representation for the managedAppOperation object.</span></span>

<span data-ttu-id="baf26-127">次の表に、managedAppOperation の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="baf26-127">The following table shows the properties that are required when you create the managedAppOperation.</span></span>

|<span data-ttu-id="baf26-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="baf26-128">Property</span></span>|<span data-ttu-id="baf26-129">種類</span><span class="sxs-lookup"><span data-stu-id="baf26-129">Type</span></span>|<span data-ttu-id="baf26-130">説明</span><span class="sxs-lookup"><span data-stu-id="baf26-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="baf26-131">displayName</span><span class="sxs-lookup"><span data-stu-id="baf26-131">displayName</span></span>|<span data-ttu-id="baf26-132">String</span><span class="sxs-lookup"><span data-stu-id="baf26-132">String</span></span>|<span data-ttu-id="baf26-133">操作名。</span><span class="sxs-lookup"><span data-stu-id="baf26-133">The operation name.</span></span>|
|<span data-ttu-id="baf26-134">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="baf26-134">lastModifiedDateTime</span></span>|<span data-ttu-id="baf26-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="baf26-135">DateTimeOffset</span></span>|<span data-ttu-id="baf26-136">アプリ操作が変更された最終時刻。</span><span class="sxs-lookup"><span data-stu-id="baf26-136">The last time the app operation was modified.</span></span>|
|<span data-ttu-id="baf26-137">state</span><span class="sxs-lookup"><span data-stu-id="baf26-137">state</span></span>|<span data-ttu-id="baf26-138">String</span><span class="sxs-lookup"><span data-stu-id="baf26-138">String</span></span>|<span data-ttu-id="baf26-139">操作の現在の状態。</span><span class="sxs-lookup"><span data-stu-id="baf26-139">The current state of the operation</span></span>|
|<span data-ttu-id="baf26-140">id</span><span class="sxs-lookup"><span data-stu-id="baf26-140">id</span></span>|<span data-ttu-id="baf26-141">String</span><span class="sxs-lookup"><span data-stu-id="baf26-141">String</span></span>|<span data-ttu-id="baf26-142">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="baf26-142">Key of the entity.</span></span>|
|<span data-ttu-id="baf26-143">version</span><span class="sxs-lookup"><span data-stu-id="baf26-143">version</span></span>|<span data-ttu-id="baf26-144">String</span><span class="sxs-lookup"><span data-stu-id="baf26-144">String</span></span>|<span data-ttu-id="baf26-145">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="baf26-145">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="baf26-146">応答</span><span class="sxs-lookup"><span data-stu-id="baf26-146">Response</span></span>
<span data-ttu-id="baf26-147">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [managedAppOperation](../resources/intune-mam-managedappoperation.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="baf26-147">If successful, this method returns a `201 Created` response code and a [managedAppOperation](../resources/intune-mam-managedappoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="baf26-148">例</span><span class="sxs-lookup"><span data-stu-id="baf26-148">Example</span></span>
### <a name="request"></a><span data-ttu-id="baf26-149">要求</span><span class="sxs-lookup"><span data-stu-id="baf26-149">Request</span></span>
<span data-ttu-id="baf26-150">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="baf26-150">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="baf26-151">応答</span><span class="sxs-lookup"><span data-stu-id="baf26-151">Response</span></span>
<span data-ttu-id="baf26-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="baf26-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



