---
title: onPremisesConditionalAccessSettings の更新
description: onPremisesConditionalAccessSettings オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1e77767900b40fc3f921d9d3ffd34fd6930bf19c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36024085"
---
# <a name="update-onpremisesconditionalaccesssettings"></a><span data-ttu-id="8187a-103">onPremisesConditionalAccessSettings の更新</span><span class="sxs-lookup"><span data-stu-id="8187a-103">Update onPremisesConditionalAccessSettings</span></span>

> <span data-ttu-id="8187a-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="8187a-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8187a-105">[onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="8187a-105">Update the properties of a [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8187a-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="8187a-106">Prerequisites</span></span>
<span data-ttu-id="8187a-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8187a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8187a-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8187a-109">Permission type</span></span>|<span data-ttu-id="8187a-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="8187a-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8187a-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8187a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="8187a-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8187a-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="8187a-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8187a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8187a-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8187a-114">Not supported.</span></span>|
|<span data-ttu-id="8187a-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8187a-115">Application</span></span>|<span data-ttu-id="8187a-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8187a-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8187a-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8187a-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/conditionalAccessSettings
```

## <a name="request-headers"></a><span data-ttu-id="8187a-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8187a-118">Request headers</span></span>
|<span data-ttu-id="8187a-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8187a-119">Header</span></span>|<span data-ttu-id="8187a-120">値</span><span class="sxs-lookup"><span data-stu-id="8187a-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8187a-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="8187a-121">Authorization</span></span>|<span data-ttu-id="8187a-122">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="8187a-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8187a-123">承諾</span><span class="sxs-lookup"><span data-stu-id="8187a-123">Accept</span></span>|<span data-ttu-id="8187a-124">application/json</span><span class="sxs-lookup"><span data-stu-id="8187a-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8187a-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="8187a-125">Request body</span></span>
<span data-ttu-id="8187a-126">要求本文で、[onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="8187a-126">In the request body, supply a JSON representation for the [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) object.</span></span>

<span data-ttu-id="8187a-127">次の表に、[onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="8187a-127">The following table shows the properties that are required when you create the [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md).</span></span>

|<span data-ttu-id="8187a-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8187a-128">Property</span></span>|<span data-ttu-id="8187a-129">型</span><span class="sxs-lookup"><span data-stu-id="8187a-129">Type</span></span>|<span data-ttu-id="8187a-130">説明</span><span class="sxs-lookup"><span data-stu-id="8187a-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8187a-131">id</span><span class="sxs-lookup"><span data-stu-id="8187a-131">id</span></span>|<span data-ttu-id="8187a-132">String</span><span class="sxs-lookup"><span data-stu-id="8187a-132">String</span></span>|<span data-ttu-id="8187a-133">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="8187a-133">Not yet documented</span></span>|
|<span data-ttu-id="8187a-134">enabled</span><span class="sxs-lookup"><span data-stu-id="8187a-134">enabled</span></span>|<span data-ttu-id="8187a-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="8187a-135">Boolean</span></span>|<span data-ttu-id="8187a-136">対象組織で、オンプレミスの条件付きアクセスが有効かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="8187a-136">Indicates if on premises conditional access is enabled for this organization</span></span>|
|<span data-ttu-id="8187a-137">includedGroups</span><span class="sxs-lookup"><span data-stu-id="8187a-137">includedGroups</span></span>|<span data-ttu-id="8187a-138">Guid コレクション</span><span class="sxs-lookup"><span data-stu-id="8187a-138">Guid collection</span></span>|<span data-ttu-id="8187a-139">オンプレミスの条件付きアクセスで対象となるユーザー グループ。</span><span class="sxs-lookup"><span data-stu-id="8187a-139">User groups that will be targeted by on premises conditional access.</span></span> <span data-ttu-id="8187a-140">これらのグループ内のユーザーすべては、管理対象のモバイル デバイスを持っており、メール アクセスに準拠している必要があります。</span><span class="sxs-lookup"><span data-stu-id="8187a-140">All users in these groups will be required to have mobile device managed and compliant for mail access.</span></span>|
|<span data-ttu-id="8187a-141">excludedGroups</span><span class="sxs-lookup"><span data-stu-id="8187a-141">excludedGroups</span></span>|<span data-ttu-id="8187a-142">Guid コレクション</span><span class="sxs-lookup"><span data-stu-id="8187a-142">Guid collection</span></span>|<span data-ttu-id="8187a-143">オンプレミスの条件付きアクセスで除外されるユーザー グループ。</span><span class="sxs-lookup"><span data-stu-id="8187a-143">User groups that will be exempt by on premises conditional access.</span></span> <span data-ttu-id="8187a-144">これらのグループ内のすべてのユーザーは、条件付きアクセス ポリシーから除外されます。</span><span class="sxs-lookup"><span data-stu-id="8187a-144">All users in these groups will be exempt from the conditional access policy.</span></span>|
|<span data-ttu-id="8187a-145">overrideDefaultRule</span><span class="sxs-lookup"><span data-stu-id="8187a-145">overrideDefaultRule</span></span>|<span data-ttu-id="8187a-146">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="8187a-146">Boolean</span></span>|<span data-ttu-id="8187a-147">デバイスでアクセスが付与されていることを確認できるようにするとき、既定のアクセス ルールを上書きします。</span><span class="sxs-lookup"><span data-stu-id="8187a-147">Override the default access rule when allowing a device to ensure access is granted.</span></span>|



## <a name="response"></a><span data-ttu-id="8187a-148">応答</span><span class="sxs-lookup"><span data-stu-id="8187a-148">Response</span></span>
<span data-ttu-id="8187a-149">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="8187a-149">If successful, this method returns a `200 OK` response code and an updated [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8187a-150">例</span><span class="sxs-lookup"><span data-stu-id="8187a-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="8187a-151">要求</span><span class="sxs-lookup"><span data-stu-id="8187a-151">Request</span></span>
<span data-ttu-id="8187a-152">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="8187a-152">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/conditionalAccessSettings
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

### <a name="response"></a><span data-ttu-id="8187a-153">応答</span><span class="sxs-lookup"><span data-stu-id="8187a-153">Response</span></span>
<span data-ttu-id="8187a-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="8187a-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



