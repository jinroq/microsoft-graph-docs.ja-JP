---
title: GroupPolicyPresentationListBox を作成します。
description: 新しい groupPolicyPresentationListBox オブジェクトを作成します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: d080fe046af88939d4c505f3848d1a7f2b1f67d3
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430343"
---
# <a name="create-grouppolicypresentationlistbox"></a><span data-ttu-id="26e73-103">GroupPolicyPresentationListBox を作成します。</span><span class="sxs-lookup"><span data-stu-id="26e73-103">Create groupPolicyPresentationListBox</span></span>

> <span data-ttu-id="26e73-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="26e73-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="26e73-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="26e73-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="26e73-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="26e73-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="26e73-107">新しい[groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="26e73-107">Create a new [groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="26e73-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="26e73-108">Prerequisites</span></span>
<span data-ttu-id="26e73-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="26e73-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="26e73-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="26e73-111">Permission type</span></span>|<span data-ttu-id="26e73-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="26e73-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="26e73-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="26e73-113">Delegated (work or school account)</span></span>|<span data-ttu-id="26e73-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="26e73-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="26e73-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="26e73-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="26e73-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="26e73-116">Not supported.</span></span>|
|<span data-ttu-id="26e73-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="26e73-117">Application</span></span>|<span data-ttu-id="26e73-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="26e73-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="26e73-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="26e73-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

## <a name="request-headers"></a><span data-ttu-id="26e73-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="26e73-120">Request headers</span></span>
|<span data-ttu-id="26e73-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="26e73-121">Header</span></span>|<span data-ttu-id="26e73-122">値</span><span class="sxs-lookup"><span data-stu-id="26e73-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="26e73-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="26e73-123">Authorization</span></span>|<span data-ttu-id="26e73-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="26e73-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="26e73-125">Accept</span><span class="sxs-lookup"><span data-stu-id="26e73-125">Accept</span></span>|<span data-ttu-id="26e73-126">application/json</span><span class="sxs-lookup"><span data-stu-id="26e73-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="26e73-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="26e73-127">Request body</span></span>
<span data-ttu-id="26e73-128">要求の本文に groupPolicyPresentationListBox オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="26e73-128">In the request body, supply a JSON representation for the groupPolicyPresentationListBox object.</span></span>

<span data-ttu-id="26e73-129">次の表は、groupPolicyPresentationListBox を作成するときに必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="26e73-129">The following table shows the properties that are required when you create the groupPolicyPresentationListBox.</span></span>

|<span data-ttu-id="26e73-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="26e73-130">Property</span></span>|<span data-ttu-id="26e73-131">型</span><span class="sxs-lookup"><span data-stu-id="26e73-131">Type</span></span>|<span data-ttu-id="26e73-132">説明</span><span class="sxs-lookup"><span data-stu-id="26e73-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="26e73-133">label</span><span class="sxs-lookup"><span data-stu-id="26e73-133">label</span></span>|<span data-ttu-id="26e73-134">String</span><span class="sxs-lookup"><span data-stu-id="26e73-134">String</span></span>|<span data-ttu-id="26e73-135">プレゼンテーションの任意のエンティティのローカライズされたテキスト ラベルです。</span><span class="sxs-lookup"><span data-stu-id="26e73-135">Localized text label for any presentation entity.</span></span> <span data-ttu-id="26e73-136">既定値は空です。</span><span class="sxs-lookup"><span data-stu-id="26e73-136">The default value is empty.</span></span> <span data-ttu-id="26e73-137">[GroupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="26e73-137">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="26e73-138">id</span><span class="sxs-lookup"><span data-stu-id="26e73-138">id</span></span>|<span data-ttu-id="26e73-139">String</span><span class="sxs-lookup"><span data-stu-id="26e73-139">String</span></span>|<span data-ttu-id="26e73-140">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="26e73-140">Key of the entity.</span></span> <span data-ttu-id="26e73-141">[GroupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="26e73-141">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="26e73-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="26e73-142">lastModifiedDateTime</span></span>|<span data-ttu-id="26e73-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="26e73-143">DateTimeOffset</span></span>|<span data-ttu-id="26e73-144">日付と時刻、エンティティが最後に修正されました。</span><span class="sxs-lookup"><span data-stu-id="26e73-144">The date and time the entity was last modified.</span></span> <span data-ttu-id="26e73-145">[GroupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="26e73-145">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="26e73-146">explicitValue</span><span class="sxs-lookup"><span data-stu-id="26e73-146">explicitValue</span></span>|<span data-ttu-id="26e73-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="26e73-147">Boolean</span></span>|<span data-ttu-id="26e73-148">True ユーザー レジストリ サブキーの値とレジストリ サブキー名を指定してくださいこのオプションを指定します。</span><span class="sxs-lookup"><span data-stu-id="26e73-148">If this option is specified true the user must specify the registry subkey value and the registry subkey name.</span></span> <span data-ttu-id="26e73-149">リスト ボックスでは、名前とデータの 2 つの列を表示します。</span><span class="sxs-lookup"><span data-stu-id="26e73-149">The list box shows two columns, one for the name and one for the data.</span></span> <span data-ttu-id="26e73-150">既定値は、false を指定します。</span><span class="sxs-lookup"><span data-stu-id="26e73-150">The default value is false.</span></span>|



## <a name="response"></a><span data-ttu-id="26e73-151">応答</span><span class="sxs-lookup"><span data-stu-id="26e73-151">Response</span></span>
<span data-ttu-id="26e73-152">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="26e73-152">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="26e73-153">例</span><span class="sxs-lookup"><span data-stu-id="26e73-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="26e73-154">要求</span><span class="sxs-lookup"><span data-stu-id="26e73-154">Request</span></span>
<span data-ttu-id="26e73-155">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="26e73-155">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
Content-type: application/json
Content-length: 125

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationListBox",
  "label": "Label value",
  "explicitValue": true
}
```

### <a name="response"></a><span data-ttu-id="26e73-156">応答</span><span class="sxs-lookup"><span data-stu-id="26e73-156">Response</span></span>
<span data-ttu-id="26e73-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="26e73-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 238

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationListBox",
  "label": "Label value",
  "id": "2e074c87-4c87-2e07-874c-072e874c072e",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "explicitValue": true
}
```




