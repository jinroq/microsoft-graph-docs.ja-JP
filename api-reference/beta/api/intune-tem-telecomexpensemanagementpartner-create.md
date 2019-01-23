---
title: telecomExpenseManagementPartner の作成
description: 新しい telecomExpenseManagementPartner オブジェクトを作成します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: d39e3b81700b95134ea2d243f6dd8920e61f48b7
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29395847"
---
# <a name="create-telecomexpensemanagementpartner"></a><span data-ttu-id="da6ac-103">telecomExpenseManagementPartner の作成</span><span class="sxs-lookup"><span data-stu-id="da6ac-103">Create telecomExpenseManagementPartner</span></span>

> <span data-ttu-id="da6ac-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="da6ac-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="da6ac-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="da6ac-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="da6ac-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="da6ac-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="da6ac-107">新しい [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="da6ac-107">Create a new [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="da6ac-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="da6ac-108">Prerequisites</span></span>
<span data-ttu-id="da6ac-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="da6ac-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="da6ac-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="da6ac-111">Permission type</span></span>|<span data-ttu-id="da6ac-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="da6ac-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="da6ac-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="da6ac-113">Delegated (work or school account)</span></span>|<span data-ttu-id="da6ac-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="da6ac-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="da6ac-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="da6ac-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="da6ac-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="da6ac-116">Not supported.</span></span>|
|<span data-ttu-id="da6ac-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="da6ac-117">Application</span></span>|<span data-ttu-id="da6ac-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="da6ac-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="da6ac-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="da6ac-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/telecomExpenseManagementPartners
```

## <a name="request-headers"></a><span data-ttu-id="da6ac-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="da6ac-120">Request headers</span></span>
|<span data-ttu-id="da6ac-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="da6ac-121">Header</span></span>|<span data-ttu-id="da6ac-122">値</span><span class="sxs-lookup"><span data-stu-id="da6ac-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="da6ac-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="da6ac-123">Authorization</span></span>|<span data-ttu-id="da6ac-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="da6ac-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="da6ac-125">Accept</span><span class="sxs-lookup"><span data-stu-id="da6ac-125">Accept</span></span>|<span data-ttu-id="da6ac-126">application/json</span><span class="sxs-lookup"><span data-stu-id="da6ac-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="da6ac-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="da6ac-127">Request body</span></span>
<span data-ttu-id="da6ac-128">要求本文で、telecomExpenseManagementPartner オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="da6ac-128">In the request body, supply a JSON representation for the telecomExpenseManagementPartner object.</span></span>

<span data-ttu-id="da6ac-129">次の表に、telecomExpenseManagementPartner の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="da6ac-129">The following table shows the properties that are required when you create the telecomExpenseManagementPartner.</span></span>

|<span data-ttu-id="da6ac-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="da6ac-130">Property</span></span>|<span data-ttu-id="da6ac-131">型</span><span class="sxs-lookup"><span data-stu-id="da6ac-131">Type</span></span>|<span data-ttu-id="da6ac-132">説明</span><span class="sxs-lookup"><span data-stu-id="da6ac-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="da6ac-133">id</span><span class="sxs-lookup"><span data-stu-id="da6ac-133">id</span></span>|<span data-ttu-id="da6ac-134">String</span><span class="sxs-lookup"><span data-stu-id="da6ac-134">String</span></span>|<span data-ttu-id="da6ac-135">TEM パートナーの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="da6ac-135">Unique identifier of the TEM partner.</span></span>|
|<span data-ttu-id="da6ac-136">displayName</span><span class="sxs-lookup"><span data-stu-id="da6ac-136">displayName</span></span>|<span data-ttu-id="da6ac-137">String</span><span class="sxs-lookup"><span data-stu-id="da6ac-137">String</span></span>|<span data-ttu-id="da6ac-138">TEM パートナーの表示名。</span><span class="sxs-lookup"><span data-stu-id="da6ac-138">Display name of the TEM partner.</span></span>|
|<span data-ttu-id="da6ac-139">url</span><span class="sxs-lookup"><span data-stu-id="da6ac-139">url</span></span>|<span data-ttu-id="da6ac-140">String</span><span class="sxs-lookup"><span data-stu-id="da6ac-140">String</span></span>|<span data-ttu-id="da6ac-141">TEM パートナーの管理用コントロール パネルの URL。管理者はここで TEM サービスを構成できます。</span><span class="sxs-lookup"><span data-stu-id="da6ac-141">URL of the TEM partner's administrative control panel, where an administrator can configure their TEM service.</span></span>|
|<span data-ttu-id="da6ac-142">appAuthorized</span><span class="sxs-lookup"><span data-stu-id="da6ac-142">appAuthorized</span></span>|<span data-ttu-id="da6ac-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="da6ac-143">Boolean</span></span>|<span data-ttu-id="da6ac-144">パートナーの AAD アプリに Intune へのアクセスが承認されているかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="da6ac-144">Whether the partner's AAD app has been authorized to access Intune.</span></span>|
|<span data-ttu-id="da6ac-145">enabled</span><span class="sxs-lookup"><span data-stu-id="da6ac-145">enabled</span></span>|<span data-ttu-id="da6ac-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="da6ac-146">Boolean</span></span>|<span data-ttu-id="da6ac-147">TEM サービスへの Intune の接続が現在有効であるか、無効であるかを指定します。</span><span class="sxs-lookup"><span data-stu-id="da6ac-147">Whether Intune's connection to the TEM service is currently enabled or disabled.</span></span>|
|<span data-ttu-id="da6ac-148">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="da6ac-148">lastConnectionDateTime</span></span>|<span data-ttu-id="da6ac-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="da6ac-149">DateTimeOffset</span></span>|<span data-ttu-id="da6ac-150">TEM パートナーによって Intune に最後に送信された要求のタイムスタンプ。</span><span class="sxs-lookup"><span data-stu-id="da6ac-150">Timestamp of the last request sent to Intune by the TEM partner.</span></span>|



## <a name="response"></a><span data-ttu-id="da6ac-151">応答</span><span class="sxs-lookup"><span data-stu-id="da6ac-151">Response</span></span>
<span data-ttu-id="da6ac-152">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="da6ac-152">If successful, this method returns a `201 Created` response code and a [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="da6ac-153">例</span><span class="sxs-lookup"><span data-stu-id="da6ac-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="da6ac-154">要求</span><span class="sxs-lookup"><span data-stu-id="da6ac-154">Request</span></span>
<span data-ttu-id="da6ac-155">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="da6ac-155">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/telecomExpenseManagementPartners
Content-type: application/json
Content-length: 248

{
  "@odata.type": "#microsoft.graph.telecomExpenseManagementPartner",
  "displayName": "Display Name value",
  "url": "Url value",
  "appAuthorized": true,
  "enabled": true,
  "lastConnectionDateTime": "2016-12-31T23:58:36.6670033-08:00"
}
```

### <a name="response"></a><span data-ttu-id="da6ac-156">応答</span><span class="sxs-lookup"><span data-stu-id="da6ac-156">Response</span></span>
<span data-ttu-id="da6ac-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="da6ac-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 297

{
  "@odata.type": "#microsoft.graph.telecomExpenseManagementPartner",
  "id": "47a3b399-b399-47a3-99b3-a34799b3a347",
  "displayName": "Display Name value",
  "url": "Url value",
  "appAuthorized": true,
  "enabled": true,
  "lastConnectionDateTime": "2016-12-31T23:58:36.6670033-08:00"
}
```




