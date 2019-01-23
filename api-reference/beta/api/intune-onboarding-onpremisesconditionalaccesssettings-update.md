---
title: onPremisesConditionalAccessSettings の更新
description: onPremisesConditionalAccessSettings オブジェクトのプロパティを更新します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: efd5ba18c958bd09e10a461350b76eb97aa56cb7
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29424036"
---
# <a name="update-onpremisesconditionalaccesssettings"></a><span data-ttu-id="2a806-103">onPremisesConditionalAccessSettings の更新</span><span class="sxs-lookup"><span data-stu-id="2a806-103">Update onPremisesConditionalAccessSettings</span></span>

> <span data-ttu-id="2a806-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="2a806-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="2a806-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2a806-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2a806-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="2a806-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2a806-107">[onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="2a806-107">Update the properties of a [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2a806-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="2a806-108">Prerequisites</span></span>
<span data-ttu-id="2a806-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2a806-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="2a806-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2a806-111">Permission type</span></span>|<span data-ttu-id="2a806-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="2a806-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2a806-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2a806-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2a806-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2a806-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="2a806-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2a806-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2a806-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2a806-116">Not supported.</span></span>|
|<span data-ttu-id="2a806-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2a806-117">Application</span></span>|<span data-ttu-id="2a806-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2a806-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2a806-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2a806-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/conditionalAccessSettings
PATCH /deviceManagement/exchangeOnPremisesPolicy/conditionalAccessSettings
```

## <a name="request-headers"></a><span data-ttu-id="2a806-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2a806-120">Request headers</span></span>
|<span data-ttu-id="2a806-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2a806-121">Header</span></span>|<span data-ttu-id="2a806-122">値</span><span class="sxs-lookup"><span data-stu-id="2a806-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2a806-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2a806-123">Authorization</span></span>|<span data-ttu-id="2a806-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="2a806-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2a806-125">Accept</span><span class="sxs-lookup"><span data-stu-id="2a806-125">Accept</span></span>|<span data-ttu-id="2a806-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2a806-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2a806-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="2a806-127">Request body</span></span>
<span data-ttu-id="2a806-128">要求本文で、[onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="2a806-128">In the request body, supply a JSON representation for the [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) object.</span></span>

<span data-ttu-id="2a806-129">次の表に、[onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="2a806-129">The following table shows the properties that are required when you create the [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md).</span></span>

|<span data-ttu-id="2a806-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2a806-130">Property</span></span>|<span data-ttu-id="2a806-131">型</span><span class="sxs-lookup"><span data-stu-id="2a806-131">Type</span></span>|<span data-ttu-id="2a806-132">説明</span><span class="sxs-lookup"><span data-stu-id="2a806-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2a806-133">id</span><span class="sxs-lookup"><span data-stu-id="2a806-133">id</span></span>|<span data-ttu-id="2a806-134">String</span><span class="sxs-lookup"><span data-stu-id="2a806-134">String</span></span>|<span data-ttu-id="2a806-135">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="2a806-135">Not yet documented</span></span>|
|<span data-ttu-id="2a806-136">enabled</span><span class="sxs-lookup"><span data-stu-id="2a806-136">enabled</span></span>|<span data-ttu-id="2a806-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="2a806-137">Boolean</span></span>|<span data-ttu-id="2a806-138">対象組織で、オンプレミスの条件付きアクセスが有効かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="2a806-138">Indicates if on premises conditional access is enabled for this organization</span></span>|
|<span data-ttu-id="2a806-139">includedGroups</span><span class="sxs-lookup"><span data-stu-id="2a806-139">includedGroups</span></span>|<span data-ttu-id="2a806-140">Guid コレクション</span><span class="sxs-lookup"><span data-stu-id="2a806-140">Guid collection</span></span>|<span data-ttu-id="2a806-141">オンプレミスの条件付きアクセスで対象となるユーザー グループ。</span><span class="sxs-lookup"><span data-stu-id="2a806-141">User groups that will be targeted by on premises conditional access.</span></span> <span data-ttu-id="2a806-142">これらのグループ内のユーザーすべては、管理対象のモバイル デバイスを持っており、メール アクセスに準拠している必要があります。</span><span class="sxs-lookup"><span data-stu-id="2a806-142">All users in these groups will be required to have mobile device managed and compliant for mail access.</span></span>|
|<span data-ttu-id="2a806-143">excludedGroups</span><span class="sxs-lookup"><span data-stu-id="2a806-143">excludedGroups</span></span>|<span data-ttu-id="2a806-144">Guid コレクション</span><span class="sxs-lookup"><span data-stu-id="2a806-144">Guid collection</span></span>|<span data-ttu-id="2a806-145">オンプレミスの条件付きアクセスで除外されるユーザー グループ。</span><span class="sxs-lookup"><span data-stu-id="2a806-145">User groups that will be exempt by on premises conditional access.</span></span> <span data-ttu-id="2a806-146">これらのグループ内のすべてのユーザーは、条件付きアクセス ポリシーから除外されます。</span><span class="sxs-lookup"><span data-stu-id="2a806-146">All users in these groups will be exempt from the conditional access policy.</span></span>|
|<span data-ttu-id="2a806-147">overrideDefaultRule</span><span class="sxs-lookup"><span data-stu-id="2a806-147">overrideDefaultRule</span></span>|<span data-ttu-id="2a806-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="2a806-148">Boolean</span></span>|<span data-ttu-id="2a806-149">デバイスでアクセスが付与されていることを確認できるようにするとき、既定のアクセス ルールを上書きします。</span><span class="sxs-lookup"><span data-stu-id="2a806-149">Override the default access rule when allowing a device to ensure access is granted.</span></span>|



## <a name="response"></a><span data-ttu-id="2a806-150">応答</span><span class="sxs-lookup"><span data-stu-id="2a806-150">Response</span></span>
<span data-ttu-id="2a806-151">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="2a806-151">If successful, this method returns a `200 OK` response code and an updated [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2a806-152">例</span><span class="sxs-lookup"><span data-stu-id="2a806-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="2a806-153">要求</span><span class="sxs-lookup"><span data-stu-id="2a806-153">Request</span></span>
<span data-ttu-id="2a806-154">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="2a806-154">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/conditionalAccessSettings
Content-type: application/json
Content-length: 275

{
  "@odata.type": "#microsoft.graph.onPremisesConditionalAccessSettings",
  "enabled": true,
  "includedGroups": [
    "77c9d466-d466-77c9-66d4-c97766d4c977"
  ],
  "excludedGroups": [
    "2a0afae4-fae4-2a0a-e4fa-0a2ae4fa0a2a"
  ],
  "overrideDefaultRule": true
}
```

### <a name="response"></a><span data-ttu-id="2a806-155">応答</span><span class="sxs-lookup"><span data-stu-id="2a806-155">Response</span></span>
<span data-ttu-id="2a806-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="2a806-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 324

{
  "@odata.type": "#microsoft.graph.onPremisesConditionalAccessSettings",
  "id": "a0efde21-de21-a0ef-21de-efa021deefa0",
  "enabled": true,
  "includedGroups": [
    "77c9d466-d466-77c9-66d4-c97766d4c977"
  ],
  "excludedGroups": [
    "2a0afae4-fae4-2a0a-e4fa-0a2ae4fa0a2a"
  ],
  "overrideDefaultRule": true
}
```




