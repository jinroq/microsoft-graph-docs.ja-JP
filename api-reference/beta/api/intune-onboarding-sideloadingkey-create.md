---
title: SideLoadingKey を作成します。
description: 新しい sideLoadingKey オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 140dc11778bad432d388f8d22173cd31cbdef915
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27974848"
---
# <a name="create-sideloadingkey"></a><span data-ttu-id="b7c8b-103">SideLoadingKey を作成します。</span><span class="sxs-lookup"><span data-stu-id="b7c8b-103">Create sideLoadingKey</span></span>

> <span data-ttu-id="b7c8b-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="b7c8b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b7c8b-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b7c8b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b7c8b-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="b7c8b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b7c8b-107">新しい[sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="b7c8b-107">Create a new [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b7c8b-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="b7c8b-108">Prerequisites</span></span>
<span data-ttu-id="b7c8b-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b7c8b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b7c8b-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b7c8b-111">Permission type</span></span>|<span data-ttu-id="b7c8b-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="b7c8b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b7c8b-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b7c8b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b7c8b-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b7c8b-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="b7c8b-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b7c8b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b7c8b-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b7c8b-116">Not supported.</span></span>|
|<span data-ttu-id="b7c8b-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b7c8b-117">Application</span></span>|<span data-ttu-id="b7c8b-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b7c8b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b7c8b-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b7c8b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/sideLoadingKeys
```

## <a name="request-headers"></a><span data-ttu-id="b7c8b-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b7c8b-120">Request headers</span></span>
|<span data-ttu-id="b7c8b-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b7c8b-121">Header</span></span>|<span data-ttu-id="b7c8b-122">値</span><span class="sxs-lookup"><span data-stu-id="b7c8b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b7c8b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b7c8b-123">Authorization</span></span>|<span data-ttu-id="b7c8b-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="b7c8b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b7c8b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b7c8b-125">Accept</span></span>|<span data-ttu-id="b7c8b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b7c8b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b7c8b-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="b7c8b-127">Request body</span></span>
<span data-ttu-id="b7c8b-128">要求の本文に sideLoadingKey オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="b7c8b-128">In the request body, supply a JSON representation for the sideLoadingKey object.</span></span>

<span data-ttu-id="b7c8b-129">次の表は、sideLoadingKey を作成するときに必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="b7c8b-129">The following table shows the properties that are required when you create the sideLoadingKey.</span></span>

|<span data-ttu-id="b7c8b-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b7c8b-130">Property</span></span>|<span data-ttu-id="b7c8b-131">種類</span><span class="sxs-lookup"><span data-stu-id="b7c8b-131">Type</span></span>|<span data-ttu-id="b7c8b-132">説明</span><span class="sxs-lookup"><span data-stu-id="b7c8b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b7c8b-133">ID</span><span class="sxs-lookup"><span data-stu-id="b7c8b-133">id</span></span>|<span data-ttu-id="b7c8b-134">String</span><span class="sxs-lookup"><span data-stu-id="b7c8b-134">String</span></span>|<span data-ttu-id="b7c8b-135">側のキーの一意の id の読み込み</span><span class="sxs-lookup"><span data-stu-id="b7c8b-135">Side Loading Key Unique Id.</span></span>|
|<span data-ttu-id="b7c8b-136">value</span><span class="sxs-lookup"><span data-stu-id="b7c8b-136">value</span></span>|<span data-ttu-id="b7c8b-137">文字列</span><span class="sxs-lookup"><span data-stu-id="b7c8b-137">String</span></span>|<span data-ttu-id="b7c8b-138">側の読み込みキー] の値は 5 列 5 行値、hiphens によって区切られています。</span><span class="sxs-lookup"><span data-stu-id="b7c8b-138">Side Loading Key Value, it is 5x5 value, seperated by hiphens.</span></span>|
|<span data-ttu-id="b7c8b-139">displayName</span><span class="sxs-lookup"><span data-stu-id="b7c8b-139">displayName</span></span>|<span data-ttu-id="b7c8b-140">String</span><span class="sxs-lookup"><span data-stu-id="b7c8b-140">String</span></span>|<span data-ttu-id="b7c8b-141">側の読み込みキー名、it プロフェッショナルの管理者に表示されます。</span><span class="sxs-lookup"><span data-stu-id="b7c8b-141">Side Loading Key Name displayed to the ITPro Admins.</span></span>|
|<span data-ttu-id="b7c8b-142">説明</span><span class="sxs-lookup"><span data-stu-id="b7c8b-142">description</span></span>|<span data-ttu-id="b7c8b-143">String</span><span class="sxs-lookup"><span data-stu-id="b7c8b-143">String</span></span>|<span data-ttu-id="b7c8b-144">側キーの読み込み中の説明は、it プロフェッショナルの管理者に表示されます.</span><span class="sxs-lookup"><span data-stu-id="b7c8b-144">Side Loading Key description displayed to the ITPro Admins..</span></span>|
|<span data-ttu-id="b7c8b-145">totalActivation</span><span class="sxs-lookup"><span data-stu-id="b7c8b-145">totalActivation</span></span>|<span data-ttu-id="b7c8b-146">Int32</span><span class="sxs-lookup"><span data-stu-id="b7c8b-146">Int32</span></span>|<span data-ttu-id="b7c8b-147">側の読み込みキー合計のアクティブ化、it プロフェッショナルの管理者に表示されます。</span><span class="sxs-lookup"><span data-stu-id="b7c8b-147">Side Loading Key Total Activation displayed to the ITPro Admins.</span></span>|
|<span data-ttu-id="b7c8b-148">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="b7c8b-148">lastUpdatedDateTime</span></span>|<span data-ttu-id="b7c8b-149">String</span><span class="sxs-lookup"><span data-stu-id="b7c8b-149">String</span></span>|<span data-ttu-id="b7c8b-150">側の読み込みキー最終更新日 it プロフェッショナルの管理者に表示されます。</span><span class="sxs-lookup"><span data-stu-id="b7c8b-150">Side Loading Key Last Updated Date displayed to the ITPro Admins.</span></span>|



## <a name="response"></a><span data-ttu-id="b7c8b-151">応答</span><span class="sxs-lookup"><span data-stu-id="b7c8b-151">Response</span></span>
<span data-ttu-id="b7c8b-152">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="b7c8b-152">If successful, this method returns a `201 Created` response code and a [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b7c8b-153">例</span><span class="sxs-lookup"><span data-stu-id="b7c8b-153">Example</span></span>
### <a name="request"></a><span data-ttu-id="b7c8b-154">要求</span><span class="sxs-lookup"><span data-stu-id="b7c8b-154">Request</span></span>
<span data-ttu-id="b7c8b-155">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b7c8b-155">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/sideLoadingKeys
Content-type: application/json
Content-length: 246

{
  "@odata.type": "#microsoft.graph.sideLoadingKey",
  "value": "Value value",
  "displayName": "Display Name value",
  "description": "Description value",
  "totalActivation": 15,
  "lastUpdatedDateTime": "Last Updated Date Time value"
}
```

### <a name="response"></a><span data-ttu-id="b7c8b-156">応答</span><span class="sxs-lookup"><span data-stu-id="b7c8b-156">Response</span></span>
<span data-ttu-id="b7c8b-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="b7c8b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





