---
title: SideLoadingKey を作成します。
description: 新しい sideLoadingKey オブジェクトを作成します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 3aa9efa7018a99f3e9f8d5f9a3d9e8569b895d0b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29400362"
---
# <a name="create-sideloadingkey"></a><span data-ttu-id="9f3a8-103">SideLoadingKey を作成します。</span><span class="sxs-lookup"><span data-stu-id="9f3a8-103">Create sideLoadingKey</span></span>

> <span data-ttu-id="9f3a8-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="9f3a8-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="9f3a8-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9f3a8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9f3a8-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="9f3a8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9f3a8-107">新しい[sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="9f3a8-107">Create a new [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9f3a8-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="9f3a8-108">Prerequisites</span></span>
<span data-ttu-id="9f3a8-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9f3a8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="9f3a8-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9f3a8-111">Permission type</span></span>|<span data-ttu-id="9f3a8-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="9f3a8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9f3a8-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9f3a8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9f3a8-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9f3a8-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="9f3a8-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9f3a8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9f3a8-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9f3a8-116">Not supported.</span></span>|
|<span data-ttu-id="9f3a8-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9f3a8-117">Application</span></span>|<span data-ttu-id="9f3a8-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9f3a8-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9f3a8-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9f3a8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/sideLoadingKeys
```

## <a name="request-headers"></a><span data-ttu-id="9f3a8-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9f3a8-120">Request headers</span></span>
|<span data-ttu-id="9f3a8-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9f3a8-121">Header</span></span>|<span data-ttu-id="9f3a8-122">値</span><span class="sxs-lookup"><span data-stu-id="9f3a8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9f3a8-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9f3a8-123">Authorization</span></span>|<span data-ttu-id="9f3a8-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="9f3a8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9f3a8-125">Accept</span><span class="sxs-lookup"><span data-stu-id="9f3a8-125">Accept</span></span>|<span data-ttu-id="9f3a8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9f3a8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9f3a8-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="9f3a8-127">Request body</span></span>
<span data-ttu-id="9f3a8-128">要求の本文に sideLoadingKey オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="9f3a8-128">In the request body, supply a JSON representation for the sideLoadingKey object.</span></span>

<span data-ttu-id="9f3a8-129">次の表は、sideLoadingKey を作成するときに必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="9f3a8-129">The following table shows the properties that are required when you create the sideLoadingKey.</span></span>

|<span data-ttu-id="9f3a8-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9f3a8-130">Property</span></span>|<span data-ttu-id="9f3a8-131">型</span><span class="sxs-lookup"><span data-stu-id="9f3a8-131">Type</span></span>|<span data-ttu-id="9f3a8-132">説明</span><span class="sxs-lookup"><span data-stu-id="9f3a8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9f3a8-133">id</span><span class="sxs-lookup"><span data-stu-id="9f3a8-133">id</span></span>|<span data-ttu-id="9f3a8-134">String</span><span class="sxs-lookup"><span data-stu-id="9f3a8-134">String</span></span>|<span data-ttu-id="9f3a8-135">側のキーの一意の id の読み込み</span><span class="sxs-lookup"><span data-stu-id="9f3a8-135">Side Loading Key Unique Id.</span></span>|
|<span data-ttu-id="9f3a8-136">value</span><span class="sxs-lookup"><span data-stu-id="9f3a8-136">value</span></span>|<span data-ttu-id="9f3a8-137">文字列</span><span class="sxs-lookup"><span data-stu-id="9f3a8-137">String</span></span>|<span data-ttu-id="9f3a8-138">側の読み込みキー] の値は 5 列 5 行値、hiphens によって区切られています。</span><span class="sxs-lookup"><span data-stu-id="9f3a8-138">Side Loading Key Value, it is 5x5 value, seperated by hiphens.</span></span>|
|<span data-ttu-id="9f3a8-139">displayName</span><span class="sxs-lookup"><span data-stu-id="9f3a8-139">displayName</span></span>|<span data-ttu-id="9f3a8-140">String</span><span class="sxs-lookup"><span data-stu-id="9f3a8-140">String</span></span>|<span data-ttu-id="9f3a8-141">側の読み込みキー名、it プロフェッショナルの管理者に表示されます。</span><span class="sxs-lookup"><span data-stu-id="9f3a8-141">Side Loading Key Name displayed to the ITPro Admins.</span></span>|
|<span data-ttu-id="9f3a8-142">説明</span><span class="sxs-lookup"><span data-stu-id="9f3a8-142">description</span></span>|<span data-ttu-id="9f3a8-143">String</span><span class="sxs-lookup"><span data-stu-id="9f3a8-143">String</span></span>|<span data-ttu-id="9f3a8-144">側キーの読み込み中の説明は、it プロフェッショナルの管理者に表示されます.</span><span class="sxs-lookup"><span data-stu-id="9f3a8-144">Side Loading Key description displayed to the ITPro Admins..</span></span>|
|<span data-ttu-id="9f3a8-145">totalActivation</span><span class="sxs-lookup"><span data-stu-id="9f3a8-145">totalActivation</span></span>|<span data-ttu-id="9f3a8-146">Int32</span><span class="sxs-lookup"><span data-stu-id="9f3a8-146">Int32</span></span>|<span data-ttu-id="9f3a8-147">側の読み込みキー合計のアクティブ化、it プロフェッショナルの管理者に表示されます。</span><span class="sxs-lookup"><span data-stu-id="9f3a8-147">Side Loading Key Total Activation displayed to the ITPro Admins.</span></span>|
|<span data-ttu-id="9f3a8-148">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="9f3a8-148">lastUpdatedDateTime</span></span>|<span data-ttu-id="9f3a8-149">String</span><span class="sxs-lookup"><span data-stu-id="9f3a8-149">String</span></span>|<span data-ttu-id="9f3a8-150">側の読み込みキー最終更新日 it プロフェッショナルの管理者に表示されます。</span><span class="sxs-lookup"><span data-stu-id="9f3a8-150">Side Loading Key Last Updated Date displayed to the ITPro Admins.</span></span>|



## <a name="response"></a><span data-ttu-id="9f3a8-151">応答</span><span class="sxs-lookup"><span data-stu-id="9f3a8-151">Response</span></span>
<span data-ttu-id="9f3a8-152">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="9f3a8-152">If successful, this method returns a `201 Created` response code and a [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9f3a8-153">例</span><span class="sxs-lookup"><span data-stu-id="9f3a8-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="9f3a8-154">要求</span><span class="sxs-lookup"><span data-stu-id="9f3a8-154">Request</span></span>
<span data-ttu-id="9f3a8-155">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="9f3a8-155">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="9f3a8-156">応答</span><span class="sxs-lookup"><span data-stu-id="9f3a8-156">Response</span></span>
<span data-ttu-id="9f3a8-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="9f3a8-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




