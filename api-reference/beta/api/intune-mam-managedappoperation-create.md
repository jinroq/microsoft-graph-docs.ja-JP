---
title: managedAppOperation の作成
description: 新しい managedAppOperation オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 994af667aadc990760d64c2f4334fc6d21eefcb9
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32530257"
---
# <a name="create-managedappoperation"></a><span data-ttu-id="790f1-103">managedAppOperation の作成</span><span class="sxs-lookup"><span data-stu-id="790f1-103">Create managedAppOperation</span></span>

> <span data-ttu-id="790f1-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="790f1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="790f1-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="790f1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="790f1-106">新しい [managedAppOperation](../resources/intune-mam-managedappoperation.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="790f1-106">Create a new [managedAppOperation](../resources/intune-mam-managedappoperation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="790f1-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="790f1-107">Prerequisites</span></span>
<span data-ttu-id="790f1-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="790f1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="790f1-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="790f1-110">Permission type</span></span>|<span data-ttu-id="790f1-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="790f1-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="790f1-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="790f1-112">Delegated (work or school account)</span></span>|<span data-ttu-id="790f1-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="790f1-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="790f1-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="790f1-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="790f1-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="790f1-115">Not supported.</span></span>|
|<span data-ttu-id="790f1-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="790f1-116">Application</span></span>|<span data-ttu-id="790f1-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="790f1-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="790f1-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="790f1-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/operations
```

## <a name="request-headers"></a><span data-ttu-id="790f1-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="790f1-119">Request headers</span></span>
|<span data-ttu-id="790f1-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="790f1-120">Header</span></span>|<span data-ttu-id="790f1-121">値</span><span class="sxs-lookup"><span data-stu-id="790f1-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="790f1-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="790f1-122">Authorization</span></span>|<span data-ttu-id="790f1-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="790f1-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="790f1-124">承諾</span><span class="sxs-lookup"><span data-stu-id="790f1-124">Accept</span></span>|<span data-ttu-id="790f1-125">application/json</span><span class="sxs-lookup"><span data-stu-id="790f1-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="790f1-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="790f1-126">Request body</span></span>
<span data-ttu-id="790f1-127">要求本文で、managedAppOperation オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="790f1-127">In the request body, supply a JSON representation for the managedAppOperation object.</span></span>

<span data-ttu-id="790f1-128">次の表に、managedAppOperation の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="790f1-128">The following table shows the properties that are required when you create the managedAppOperation.</span></span>

|<span data-ttu-id="790f1-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="790f1-129">Property</span></span>|<span data-ttu-id="790f1-130">型</span><span class="sxs-lookup"><span data-stu-id="790f1-130">Type</span></span>|<span data-ttu-id="790f1-131">説明</span><span class="sxs-lookup"><span data-stu-id="790f1-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="790f1-132">displayName</span><span class="sxs-lookup"><span data-stu-id="790f1-132">displayName</span></span>|<span data-ttu-id="790f1-133">String</span><span class="sxs-lookup"><span data-stu-id="790f1-133">String</span></span>|<span data-ttu-id="790f1-134">操作名。</span><span class="sxs-lookup"><span data-stu-id="790f1-134">The operation name.</span></span>|
|<span data-ttu-id="790f1-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="790f1-135">lastModifiedDateTime</span></span>|<span data-ttu-id="790f1-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="790f1-136">DateTimeOffset</span></span>|<span data-ttu-id="790f1-137">アプリ操作が変更された最終時刻。</span><span class="sxs-lookup"><span data-stu-id="790f1-137">The last time the app operation was modified.</span></span>|
|<span data-ttu-id="790f1-138">state</span><span class="sxs-lookup"><span data-stu-id="790f1-138">state</span></span>|<span data-ttu-id="790f1-139">String</span><span class="sxs-lookup"><span data-stu-id="790f1-139">String</span></span>|<span data-ttu-id="790f1-140">操作の現在の状態。</span><span class="sxs-lookup"><span data-stu-id="790f1-140">The current state of the operation</span></span>|
|<span data-ttu-id="790f1-141">id</span><span class="sxs-lookup"><span data-stu-id="790f1-141">id</span></span>|<span data-ttu-id="790f1-142">String</span><span class="sxs-lookup"><span data-stu-id="790f1-142">String</span></span>|<span data-ttu-id="790f1-143">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="790f1-143">Key of the entity.</span></span>|
|<span data-ttu-id="790f1-144">version</span><span class="sxs-lookup"><span data-stu-id="790f1-144">version</span></span>|<span data-ttu-id="790f1-145">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="790f1-145">String</span></span>|<span data-ttu-id="790f1-146">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="790f1-146">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="790f1-147">応答</span><span class="sxs-lookup"><span data-stu-id="790f1-147">Response</span></span>
<span data-ttu-id="790f1-148">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [managedAppOperation](../resources/intune-mam-managedappoperation.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="790f1-148">If successful, this method returns a `201 Created` response code and a [managedAppOperation](../resources/intune-mam-managedappoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="790f1-149">例</span><span class="sxs-lookup"><span data-stu-id="790f1-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="790f1-150">要求</span><span class="sxs-lookup"><span data-stu-id="790f1-150">Request</span></span>
<span data-ttu-id="790f1-151">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="790f1-151">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/operations
Content-type: application/json
Content-length: 159

{
  "@odata.type": "#microsoft.graph.managedAppOperation",
  "displayName": "Display Name value",
  "state": "State value",
  "version": "Version value"
}
```

### <a name="response"></a><span data-ttu-id="790f1-152">応答</span><span class="sxs-lookup"><span data-stu-id="790f1-152">Response</span></span>
<span data-ttu-id="790f1-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="790f1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





