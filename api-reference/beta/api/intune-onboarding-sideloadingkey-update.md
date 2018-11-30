---
title: SideLoadingKey を更新します。
description: SideLoadingKey オブジェクトのプロパティを更新します。
ms.openlocfilehash: 5c9071a47726f602fcd07fd47341c70f7b4b2f38
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27072193"
---
# <a name="update-sideloadingkey"></a><span data-ttu-id="662d4-103">SideLoadingKey を更新します。</span><span class="sxs-lookup"><span data-stu-id="662d4-103">Update sideLoadingKey</span></span>

> <span data-ttu-id="662d4-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="662d4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="662d4-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="662d4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="662d4-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="662d4-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="662d4-107">[SideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="662d4-107">Update the properties of a [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="662d4-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="662d4-108">Prerequisites</span></span>
<span data-ttu-id="662d4-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="662d4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="662d4-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="662d4-111">Permission type</span></span>|<span data-ttu-id="662d4-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="662d4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="662d4-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="662d4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="662d4-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="662d4-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="662d4-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="662d4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="662d4-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="662d4-116">Not supported.</span></span>|
|<span data-ttu-id="662d4-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="662d4-117">Application</span></span>|<span data-ttu-id="662d4-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="662d4-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="662d4-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="662d4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/sideLoadingKeys/{sideLoadingKeyId}
```

## <a name="request-headers"></a><span data-ttu-id="662d4-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="662d4-120">Request headers</span></span>
|<span data-ttu-id="662d4-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="662d4-121">Header</span></span>|<span data-ttu-id="662d4-122">値</span><span class="sxs-lookup"><span data-stu-id="662d4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="662d4-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="662d4-123">Authorization</span></span>|<span data-ttu-id="662d4-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="662d4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="662d4-125">Accept</span><span class="sxs-lookup"><span data-stu-id="662d4-125">Accept</span></span>|<span data-ttu-id="662d4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="662d4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="662d4-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="662d4-127">Request body</span></span>
<span data-ttu-id="662d4-128">要求の本文に[sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="662d4-128">In the request body, supply a JSON representation for the [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) object.</span></span>

<span data-ttu-id="662d4-129">[SideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="662d4-129">The following table shows the properties that are required when you create the [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md).</span></span>

|<span data-ttu-id="662d4-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="662d4-130">Property</span></span>|<span data-ttu-id="662d4-131">型</span><span class="sxs-lookup"><span data-stu-id="662d4-131">Type</span></span>|<span data-ttu-id="662d4-132">説明</span><span class="sxs-lookup"><span data-stu-id="662d4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="662d4-133">id</span><span class="sxs-lookup"><span data-stu-id="662d4-133">id</span></span>|<span data-ttu-id="662d4-134">String</span><span class="sxs-lookup"><span data-stu-id="662d4-134">String</span></span>|<span data-ttu-id="662d4-135">側のキーの一意の id の読み込み</span><span class="sxs-lookup"><span data-stu-id="662d4-135">Side Loading Key Unique Id.</span></span>|
|<span data-ttu-id="662d4-136">value</span><span class="sxs-lookup"><span data-stu-id="662d4-136">value</span></span>|<span data-ttu-id="662d4-137">文字列</span><span class="sxs-lookup"><span data-stu-id="662d4-137">String</span></span>|<span data-ttu-id="662d4-138">側の読み込みキー] の値は 5 列 5 行値、hiphens によって区切られています。</span><span class="sxs-lookup"><span data-stu-id="662d4-138">Side Loading Key Value, it is 5x5 value, seperated by hiphens.</span></span>|
|<span data-ttu-id="662d4-139">displayName</span><span class="sxs-lookup"><span data-stu-id="662d4-139">displayName</span></span>|<span data-ttu-id="662d4-140">String</span><span class="sxs-lookup"><span data-stu-id="662d4-140">String</span></span>|<span data-ttu-id="662d4-141">側の読み込みキー名、it プロフェッショナルの管理者に表示されます。</span><span class="sxs-lookup"><span data-stu-id="662d4-141">Side Loading Key Name displayed to the ITPro Admins.</span></span>|
|<span data-ttu-id="662d4-142">説明</span><span class="sxs-lookup"><span data-stu-id="662d4-142">description</span></span>|<span data-ttu-id="662d4-143">String</span><span class="sxs-lookup"><span data-stu-id="662d4-143">String</span></span>|<span data-ttu-id="662d4-144">側キーの読み込み中の説明は、it プロフェッショナルの管理者に表示されます.</span><span class="sxs-lookup"><span data-stu-id="662d4-144">Side Loading Key description displayed to the ITPro Admins..</span></span>|
|<span data-ttu-id="662d4-145">totalActivation</span><span class="sxs-lookup"><span data-stu-id="662d4-145">totalActivation</span></span>|<span data-ttu-id="662d4-146">Int32</span><span class="sxs-lookup"><span data-stu-id="662d4-146">Int32</span></span>|<span data-ttu-id="662d4-147">側の読み込みキー合計のアクティブ化、it プロフェッショナルの管理者に表示されます。</span><span class="sxs-lookup"><span data-stu-id="662d4-147">Side Loading Key Total Activation displayed to the ITPro Admins.</span></span>|
|<span data-ttu-id="662d4-148">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="662d4-148">lastUpdatedDateTime</span></span>|<span data-ttu-id="662d4-149">String</span><span class="sxs-lookup"><span data-stu-id="662d4-149">String</span></span>|<span data-ttu-id="662d4-150">側の読み込みキー最終更新日 it プロフェッショナルの管理者に表示されます。</span><span class="sxs-lookup"><span data-stu-id="662d4-150">Side Loading Key Last Updated Date displayed to the ITPro Admins.</span></span>|



## <a name="response"></a><span data-ttu-id="662d4-151">応答</span><span class="sxs-lookup"><span data-stu-id="662d4-151">Response</span></span>
<span data-ttu-id="662d4-152">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="662d4-152">If successful, this method returns a `200 OK` response code and an updated [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="662d4-153">例</span><span class="sxs-lookup"><span data-stu-id="662d4-153">Example</span></span>
### <a name="request"></a><span data-ttu-id="662d4-154">要求</span><span class="sxs-lookup"><span data-stu-id="662d4-154">Request</span></span>
<span data-ttu-id="662d4-155">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="662d4-155">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/sideLoadingKeys/{sideLoadingKeyId}
Content-type: application/json
Content-length: 193

{
  "value": "Value value",
  "displayName": "Display Name value",
  "description": "Description value",
  "totalActivation": 15,
  "lastUpdatedDateTime": "Last Updated Date Time value"
}
```

### <a name="response"></a><span data-ttu-id="662d4-156">応答</span><span class="sxs-lookup"><span data-stu-id="662d4-156">Response</span></span>
<span data-ttu-id="662d4-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="662d4-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 295

{
  "@odata.type": "#microsoft.graph.sideLoadingKey",
  "id": "21c4a3ff-a3ff-21c4-ffa3-c421ffa3c421",
  "value": "Value value",
  "displayName": "Display Name value",
  "description": "Description value",
  "totalActivation": 15,
  "lastUpdatedDateTime": "Last Updated Date Time value"
}
```





