---
title: Azure AD アクセスを確認します。
description: Azure AD を使用するユーザーのアクセス権の陣のレビューを 1 回限りまたは定期的なアクセスを構成するのにはレビューにアクセスします。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 212af4ad8519f7ec54fb56ceffee0a0d4de16027
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516414"
---
# <a name="azure-ad-access-reviews"></a>Azure AD アクセスを確認します。

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[Azure AD アクセスの確認](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-azure-ad-controls-access-reviews-overview)を使用 1 回のみを構成するか、定期的なアクセスをユーザーのアクセス権の認証の確認します。

アクセスのための一般的な顧客シナリオは、グループ メンバーシップの確認およびアプリケーションへのアクセス。
   
- お客様は、確認し、アプリケーションへのアクセスのアクセスのレビューとグループのメンバーシップを使用してゲスト ユーザーのアクセスを認定できます。 レビュー担当者は、効率的にアクセスする必要があります来園者に続きがあるかどうかを決定するのには提供されている情報を使用できます。
      
- 顧客がアプリケーションへの従業員のアクセスを認定してグループ メンバーシップのアクセス確認をします。
   
- お客様は、コンプライアンスやリスクに敏感なアプリケーションのレビューを追跡するために、組織に関連付けられているプログラムに、レビューのアクセス制御を収集できます。

Azure AD グローバル管理者ロールまたは Azure サブスクリプション ロール ロールに割り当てられているを確認し、管理者のユーザーのロールの割り当てを保証するお客様に関連する機能もあります。  [Azure AD 特権 Id 管理](privilegedidentitymanagement-root.md)では、この機能が含まれます。

Azure AD プレミアム P2 で、API を含む、アクセスのレビュー機能が含まれていることに注意してください。 

## <a name="methods"></a>メソッド

Azure AD で提供されているメソッドの一覧をここではレビューにアクセスします。  

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[AccessReview を取得します。](../api/accessreview-get.md) |   [accessReview](accessreview.md) |   特定の id を持つ、アクセス確認を取得します。 |
|[AccessReview を作成します。](../api/accessreview-create.md) | [accessReview](accessreview.md) |   新しい accessReview を作成します。 |
|[AccessReview を削除します。](../api/accessreview-delete.md) | なし。   | AccessReview を削除します。 |
|[AccessReview を更新します。](../api/accessreview-update.md) | [accessReview](accessreview.md) | AccessReview を更新します。 |
|[AccessReview の校閲者の一覧](../api/accessreview-listreviewers.md) |      コレクションを[割り当てられていません](useridentity.md)| AccessReview のレビュー担当者を取得します。 |
|[AccessReview の校閲者を追加します。](../api/accessreview-addreviewer.md) |      なし。   |   AccessReview には、レビュー担当者を追加します。 |
|[AccessReview のレビュー担当者を削除します。](../api/accessreview-removereviewer.md) | なし。  |   AccessReview からレビュー担当者を削除します。 |
|[リストの accessReview の決定](../api/accessreview-listdecisions.md) |      [accessReviewDecision](accessreviewdecision.md)コレクション| AccessReview の決定を取得します。|
|[マイ accessReview の決定事項を表示します。](../api/accessreview-listmydecisions.md) |     [accessReviewDecision](accessreviewdecision.md)コレクション| 参照者、accessReview の自分の意思決定を取得します。|
|[AccessReview アラームを送信します。](../api/accessreview-sendreminder.md) |        なし。   |   AccessReview のレビュー担当者に通知を送信します。 |
|[AccessReview を停止します。](../api/accessreview-stop.md) |     なし。   |   AccessReview を停止します。 |
|[リセット accessReview 決定](../api/accessreview-reset.md) |     なし。   |   進行中の accessReview の決定をリセットします。|
|[AccessReview の決定を適用します。](../api/accessreview-apply.md) |     なし。   |   完了した accessReview からの決定を適用します。|
|[リスト businessFlowTemplates](../api/businessflowtemplate-list.md) | [businessFlowTemplate](businessflowtemplate.md)コレクション| レビューにアクセスする適切なビジネス フローのテンプレートを取得します。|
|[プログラムを作成します。](../api/program-create.md) |   [プログラム](program.md)   |   新しいプログラムを作成します。|
|[プログラムを削除します。](../api/program-delete.md) |   なし。   |   プログラムを削除します。|
|[プログラムを一覧表示](../api/program-list.md) |  [プログラム](program.md)のコレクション|   すべてのプログラムのコレクションを取得します。|
|[プログラムのリスト programControls](../api/program-listcontrols.md) |      [デバッギング](programcontrol.md)コレクション| プログラムのコントロールのコレクションを取得します。|
|[更新プログラム](../api/program-update.md) |   [プログラム](program.md)|  プログラムを更新します。|
|[デバッギングを作成します。](../api/programcontrol-create.md) |     [デバッギング](programcontrol.md) |   デバッギングをプログラムに追加します。|
|[デバッギングを削除します。](../api/programcontrol-delete.md) |     なし。   |   デバッギングをプログラムから削除します。|
|[リスト programControls](../api/programcontrol-list.md) | [デバッギング](programcontrol.md)コレクション| テナント内のすべてのプログラム間でコントロールを一覧表示します。|
|[リスト programControlTypes](../api/programcontroltype-list.md) | [programControlType](programcontroltype.md)コレクション| プログラムのコントロールの種類を一覧表示します。 |


## <a name="see-also"></a>関連項目

- [管理者が Azure AD にアクセスできるユーザーのアクセスを管理する方法を確認します。](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-azure-ad-controls-manage-user-access-with-access-reviews)
- [Azure AD のアクセス権を持つゲスト アクセスを管理者が管理できる方法を確認します。](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-azure-ad-controls-manage-guest-access-with-access-reviews)
- [管理者がプログラムを管理し、Azure AD のコントロールがレビューをアクセスする方法](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-azure-ad-controls-manage-programs-controls)


<!--
{
  "type": "#page.annotation",
  "description": "Service root",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/accessreviews-root.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
