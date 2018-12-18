---
title: deviceCategory の作成
description: 新しい deviceCategory オブジェクトを作成します。
author: tfitzmac
ms.openlocfilehash: a6481784721396bc6d7011fb91ea18e8119390bb
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27307302"
---
# <a name="create-devicecategory"></a><span data-ttu-id="42271-103">deviceCategory の作成</span><span class="sxs-lookup"><span data-stu-id="42271-103">Create deviceCategory</span></span>

> <span data-ttu-id="42271-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="42271-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="42271-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="42271-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="42271-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="42271-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="42271-107">新しい [deviceCategory](../resources/intune-shared-devicecategory.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="42271-107">Create a new [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="42271-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="42271-108">Prerequisites</span></span>

<span data-ttu-id="42271-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="42271-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="42271-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="42271-111">Permission type</span></span>|<span data-ttu-id="42271-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="42271-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="42271-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="42271-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="42271-114">&nbsp;&nbsp; **契約時**</span><span class="sxs-lookup"><span data-stu-id="42271-114">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="42271-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="42271-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="42271-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="42271-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="42271-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="42271-117">Not supported.</span></span>|
|<span data-ttu-id="42271-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="42271-118">Application</span></span>|<span data-ttu-id="42271-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="42271-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="42271-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="42271-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCategories
```

## <a name="request-headers"></a><span data-ttu-id="42271-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="42271-121">Request headers</span></span>

|<span data-ttu-id="42271-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="42271-122">Header</span></span>|<span data-ttu-id="42271-123">値</span><span class="sxs-lookup"><span data-stu-id="42271-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="42271-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="42271-124">Authorization</span></span>|<span data-ttu-id="42271-125">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="42271-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="42271-126">Accept</span><span class="sxs-lookup"><span data-stu-id="42271-126">Accept</span></span>|<span data-ttu-id="42271-127">application/json</span><span class="sxs-lookup"><span data-stu-id="42271-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="42271-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="42271-128">Request body</span></span>

<span data-ttu-id="42271-129">要求本文で、deviceCategory オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="42271-129">In the request body, supply a JSON representation for the deviceCategory object.</span></span>

<span data-ttu-id="42271-130">次の表に、deviceCategory の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="42271-130">The following table shows the properties that are required when you create the deviceCategory.</span></span>

|<span data-ttu-id="42271-131">プロパティ</span><span class="sxs-lookup"><span data-stu-id="42271-131">Property</span></span>|<span data-ttu-id="42271-132">種類</span><span class="sxs-lookup"><span data-stu-id="42271-132">Type</span></span>|<span data-ttu-id="42271-133">説明</span><span class="sxs-lookup"><span data-stu-id="42271-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="42271-134">ID</span><span class="sxs-lookup"><span data-stu-id="42271-134">id</span></span>|<span data-ttu-id="42271-135">String</span><span class="sxs-lookup"><span data-stu-id="42271-135">String</span></span>|<span data-ttu-id="42271-136">デバイス カテゴリの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="42271-136">Unique identifier for the device category.</span></span> <span data-ttu-id="42271-137">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="42271-137">Read-only.</span></span>|
|<span data-ttu-id="42271-138">**Obboarding**</span><span class="sxs-lookup"><span data-stu-id="42271-138">**Obboarding**</span></span>|
|<span data-ttu-id="42271-139">説明</span><span class="sxs-lookup"><span data-stu-id="42271-139">description</span></span>|<span data-ttu-id="42271-140">String</span><span class="sxs-lookup"><span data-stu-id="42271-140">String</span></span>|<span data-ttu-id="42271-141">デバイス カテゴリに関するオプションの説明。</span><span class="sxs-lookup"><span data-stu-id="42271-141">Optional description for the device category.</span></span>|
|<span data-ttu-id="42271-142">displayName</span><span class="sxs-lookup"><span data-stu-id="42271-142">displayName</span></span>|<span data-ttu-id="42271-143">String</span><span class="sxs-lookup"><span data-stu-id="42271-143">String</span></span>|<span data-ttu-id="42271-144">デバイス カテゴリの表示名。</span><span class="sxs-lookup"><span data-stu-id="42271-144">Display name for the device category.</span></span>|

## <a name="response"></a><span data-ttu-id="42271-145">応答</span><span class="sxs-lookup"><span data-stu-id="42271-145">Response</span></span>

<span data-ttu-id="42271-146">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [deviceCategory](../resources/intune-shared-devicecategory.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="42271-146">If successful, this method returns a `201 Created` response code and a [deviceCategory](../resources/intune-shared-devicecategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="42271-147">例</span><span class="sxs-lookup"><span data-stu-id="42271-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="42271-148">要求</span><span class="sxs-lookup"><span data-stu-id="42271-148">Request</span></span>

<span data-ttu-id="42271-149">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="42271-149">Here is an example of the request.</span></span>

``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCategories
Content-type: application/json
Content-length: 135

{
  "@odata.type": "#microsoft.graph.deviceCategory",
  "displayName": "Display Name value",
  "description": "Description value"
}
```

### <a name="response"></a><span data-ttu-id="42271-150">応答</span><span class="sxs-lookup"><span data-stu-id="42271-150">Response</span></span>

<span data-ttu-id="42271-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="42271-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 184

{
  "@odata.type": "#microsoft.graph.deviceCategory",
  "id": "f881b841-b841-f881-41b8-81f841b881f8",
  "displayName": "Display Name value",
  "description": "Description value"
}
```



