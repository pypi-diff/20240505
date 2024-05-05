# Comparing `tmp/ynab_split_budget-1.0.0.tar.gz` & `tmp/ynab_split_budget-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ynab_split_budget-1.0.0.tar", max compression
+gzip compressed data, was "ynab_split_budget-1.0.1.tar", max compression
```

## Comparing `ynab_split_budget-1.0.0.tar` & `ynab_split_budget-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0    35148 2024-05-02 06:31:54.663098 ynab_split_budget-1.0.0/LICENSE
--rw-r--r--   0        0        0     5110 2024-05-02 06:31:54.663098 ynab_split_budget-1.0.0/README.md
--rw-r--r--   0        0        0      842 2024-05-02 06:32:08.895079 ynab_split_budget-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      175 2024-05-02 06:31:54.663098 ynab_split_budget-1.0.0/ynabsplitbudget/__init__.py
--rw-r--r--   0        0        0     2449 2024-05-02 06:31:54.663098 ynab_split_budget-1.0.0/ynabsplitbudget/__main__.py
--rw-r--r--   0        0        0     2215 2024-05-02 06:31:54.663098 ynab_split_budget-1.0.0/ynabsplitbudget/adjusters.py
--rw-r--r--   0        0        0     4230 2024-05-02 06:31:54.663098 ynab_split_budget-1.0.0/ynabsplitbudget/client.py
--rw-r--r--   0        0        0        0 2024-05-02 06:31:54.663098 ynab_split_budget-1.0.0/ynabsplitbudget/models/__init__.py
--rw-r--r--   0        0        0      194 2024-05-02 06:31:54.663098 ynab_split_budget-1.0.0/ynabsplitbudget/models/account.py
--rw-r--r--   0        0        0      105 2024-05-02 06:31:54.663098 ynab_split_budget-1.0.0/ynabsplitbudget/models/category.py
--rw-r--r--   0        0        0      247 2024-05-02 06:31:54.663098 ynab_split_budget-1.0.0/ynabsplitbudget/models/exception.py
--rw-r--r--   0        0        0      503 2024-05-02 06:31:54.663098 ynab_split_budget-1.0.0/ynabsplitbudget/models/transaction.py
--rw-r--r--   0        0        0     1741 2024-05-02 06:31:54.663098 ynab_split_budget-1.0.0/ynabsplitbudget/models/user.py
--rw-r--r--   0        0        0      945 2024-05-02 06:31:54.663098 ynab_split_budget-1.0.0/ynabsplitbudget/splitparser.py
--rw-r--r--   0        0        0     2634 2024-05-02 06:31:54.663098 ynab_split_budget-1.0.0/ynabsplitbudget/syncrepository.py
--rw-r--r--   0        0        0     2216 2024-05-02 06:31:54.663098 ynab_split_budget-1.0.0/ynabsplitbudget/transactionbuilder.py
--rw-r--r--   0        0        0     5325 2024-05-02 06:31:54.663098 ynab_split_budget-1.0.0/ynabsplitbudget/ynabsplitbudget.py
--rw-r--r--   0        0        0     5929 1970-01-01 00:00:00.000000 ynab_split_budget-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0    35148 2024-05-05 05:38:40.934880 ynab_split_budget-1.0.1/LICENSE
+-rw-r--r--   0        0        0     5219 2024-05-05 05:38:40.934880 ynab_split_budget-1.0.1/README.md
+-rw-r--r--   0        0        0      842 2024-05-05 05:39:05.338922 ynab_split_budget-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0      175 2024-05-05 05:38:40.934880 ynab_split_budget-1.0.1/ynabsplitbudget/__init__.py
+-rw-r--r--   0        0        0     2487 2024-05-05 05:38:40.934880 ynab_split_budget-1.0.1/ynabsplitbudget/__main__.py
+-rw-r--r--   0        0        0     2288 2024-05-05 05:38:40.934880 ynab_split_budget-1.0.1/ynabsplitbudget/adjusters.py
+-rw-r--r--   0        0        0     4336 2024-05-05 05:38:40.934880 ynab_split_budget-1.0.1/ynabsplitbudget/client.py
+-rw-r--r--   0        0        0        0 2024-05-05 05:38:40.934880 ynab_split_budget-1.0.1/ynabsplitbudget/models/__init__.py
+-rw-r--r--   0        0        0      194 2024-05-05 05:38:40.934880 ynab_split_budget-1.0.1/ynabsplitbudget/models/account.py
+-rw-r--r--   0        0        0      105 2024-05-05 05:38:40.934880 ynab_split_budget-1.0.1/ynabsplitbudget/models/category.py
+-rw-r--r--   0        0        0      247 2024-05-05 05:38:40.934880 ynab_split_budget-1.0.1/ynabsplitbudget/models/exception.py
+-rw-r--r--   0        0        0      503 2024-05-05 05:38:40.934880 ynab_split_budget-1.0.1/ynabsplitbudget/models/transaction.py
+-rw-r--r--   0        0        0     1741 2024-05-05 05:38:40.934880 ynab_split_budget-1.0.1/ynabsplitbudget/models/user.py
+-rw-r--r--   0        0        0      945 2024-05-05 05:38:40.934880 ynab_split_budget-1.0.1/ynabsplitbudget/splitparser.py
+-rw-r--r--   0        0        0     2736 2024-05-05 05:38:40.934880 ynab_split_budget-1.0.1/ynabsplitbudget/syncrepository.py
+-rw-r--r--   0        0        0     2216 2024-05-05 05:38:40.934880 ynab_split_budget-1.0.1/ynabsplitbudget/transactionbuilder.py
+-rw-r--r--   0        0        0     4187 2024-05-05 05:38:40.934880 ynab_split_budget-1.0.1/ynabsplitbudget/ynabsplitbudget.py
+-rw-r--r--   0        0        0     6038 1970-01-01 00:00:00.000000 ynab_split_budget-1.0.1/PKG-INFO
```

### Comparing `ynab_split_budget-1.0.0/LICENSE` & `ynab_split_budget-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ynab_split_budget-1.0.0/README.md` & `ynab_split_budget-1.0.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,28 @@
+Metadata-Version: 2.1
+Name: ynab-split-budget
+Version: 1.0.1
+Summary: Library to split and share You Need A Budget (YNAB) transactions between two budgets
+License: MIT
+Author: Daniel Basta
+Author-email: ynab@basta.info
+Requires-Python: >=3.8,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: pyyaml (>=6.0,<7.0)
+Requires-Dist: requests (>=2.28,<3.0)
+Requires-Dist: ynab-transaction-adjuster (>=2.0.0,<3.0.0)
+Description-Content-Type: text/markdown
+
 # ynab-split-budget
 
 [![GitHub Release](https://img.shields.io/github/release/dnbasta/ynab-split-budget?style=flat)]() 
 [![Github Release](https://img.shields.io/maintenance/yes/2100)]()
 [![Monthly downloads](https://img.shields.io/pypi/dm/ynab-split-budget)]()
 
 This library enables cost sharing across two YNAB budgets. It requires two dedicated accounts in each budget to which
@@ -44,27 +65,32 @@
                account_id='<account_id', flag_color='<flag_color>')
 
 split_budget = YnabSplitBudget(user=user, partner=partner)
 ```
 ### 3. Split transactions
 Call the `split()` method of the instance. It will split flagged transactions in the budget into a subtransaction with
 the original category and a transfer to the split account. By default, the transfer transactions will show up as 
-uncleared in the split account. The optional `clear` parameter allows to automatically clear the transactions in 
-the split account. The function returns the updated transactions after applying the split.
+uncleared in the split account.
 ```py
 split_budget.split()
 ```
 
 ### 4. Push new splits to partner split account
 Calling the `push()` function will insert new transactions from user split account into split account of partner to keep
-both accounts in sync. By default, the function will compare and insert transactions of the last 30 days. Optionally it 
+both accounts in sync. By default, the function will only consider cleared transactions. This is in general a safer 
+option as it forces users to manually check and clear transactions in the split account. However, it makes running the 
+whole functionality automatically cumbersome, hence the function takes an optional `include_uncleared` parameter which, 
+if set to `True`, makes it also consider uncleared transactions. 
+Additionally by default, the function will compare and insert transactions of the last 30 days. Optionally it 
 takes a `since` parameter in the form of `datetime.date` to set a timeframe different from 30 days. 
 
 ```py
 split_budget.push()
+# or optionally with considering uncleared transactions as well
+split_budget.push(include_uncleared=True)
 ```
 ## Advanced Usage
 ### Check Balances
 The `raise_on_balances_off()` function compares the cleared balances in both split accounts. If they don't match it 
 will raise a `BalancesDontMatch` error which includes the values of the balances.
 ```py
 split_budget.raise_on_balances_off()
@@ -73,20 +99,14 @@
 The `delete_orphans()` function deletes orphaned transactions in the partner split account, which don't have a 
 corresponding transaction in the user split account any more. It does return a list with the deleted transactions. 
 By default, the function compares transactions of the last 30 days. Optionally it takes a `since` parameter in the 
 form of `datetime.date` to set a timeframe different from 30 days.
 ```py
 split_budget.delete_orphans()
 ```
-### Reconcile split account
-The `reconcile()` function allows to reconcile the split account. It does check if the balances match before reconciling
-and will an `BalancesDontMatch` error if they don't.
-```py 
-split_budget.reconcile()
-```
 
 ### Show Logs
 The library logs information about the result of the methods at the 'INFO' level. The logs can be made visible by 
 importing the logging module and set it to the level `INFO`. The logger itself can also be accessed via the `logger` 
 attribute of the instance.
 ```py
 import logging
@@ -98,7 +118,8 @@
 ```bash
 $ python -m ynabsplitbudget -u <path/user.yaml> -p <path/partner.yaml> --split
 ```
 For a complete list of available bash options please use
 ```bash
 $ python -m ynabsplitbudget -h | -- help
 ```
+
```

### Comparing `ynab_split_budget-1.0.0/pyproject.toml` & `ynab_split_budget-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry-core.masonry.api"
 
 [tool.poetry]
 name = "ynab-split-budget"
-version = "1.0.0"
+version = "1.0.1"
 authors = ["Daniel Basta <ynab@basta.info>"]
 description = "Library to split and share You Need A Budget (YNAB) transactions between two budgets"
 readme = "README.md"
 license = 'MIT'
 packages = [{include = 'ynabsplitbudget'}]
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `ynab_split_budget-1.0.0/ynabsplitbudget/__main__.py` & `ynab_split_budget-1.0.1/ynabsplitbudget/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,34 +16,34 @@
 
 if __name__ == '__main__':
 	parser = argparse.ArgumentParser(formatter_class=argparse.ArgumentDefaultsHelpFormatter,
 									 usage='ynabsplitbudget [-u | --user] <path/user.yaml> '
 										   '[-p | --partner] <path/partner.yaml> '
 										   '[-s | --split] '
 										   '[-i | --push] '
+										   '[-iu | --push-uncleared] '
 										   '[-b | --balances]'
 										   '[-d | --delete-orphans]'
-										   '[-r | --reconcile]'
 										   '[--since "YYYY-mm-dd"]')
 	parser.add_argument("-u", "--user", type=str, required=True,
 						help="path of config YAML to use for user")
 	parser.add_argument("-p", "--partner", type=str, required=True,
 						help="path of config YAML to use for partner")
 	parser.add_argument("-s", "--split", action="store_true",
 						help="split transactions from account")
 	parser.add_argument("-i", "--push", action="store_true",
 						help="push split transactions to partner account")
 	parser.add_argument("-b", "--balances", action="store_true",
 						help="raise error if balances of the two accounts don't match")
 	parser.add_argument("-d", "--delete-orphans", action="store_true",
 						help="deletes orphaned transactions in partner account")
-	parser.add_argument("-r", "--reconcile", action="store_true",
-						help="reconciles account if balance matches with partner account")
 	parser.add_argument("--since", type=str,
 						help='provide optional date if library should use something else than 30 days default')
+	parser.add_argument('-iu', "--push-uncleared", type=str,
+						help='push split transactions to partner account including uncleared transactions')
 
 	args = parser.parse_args()
 
 	warnings.showwarning = custom_warn
 	user = User.from_yaml(args.user)
 	partner = User.from_yaml(args.partner)
 	ysb = YnabSplitBudget(user=user, partner=partner)
@@ -56,15 +56,15 @@
 	else:
 		since = None
 
 	if args.split:
 		ysb.split()
 	if args.push:
 		ysb.push(since=since)
+	elif args.push_uncleared:
+		ysb.push(since=since, include_uncleared=True)
 	if args.delete_orphans:
 		ysb.delete_orphans(since=since)
-	if args.balances or args.reconcile:
+	if args.balances:
 		ysb.raise_on_balances_off()
-	if args.reconcile:
-		ysb.reconcile()
```

### Comparing `ynab_split_budget-1.0.0/ynabsplitbudget/adjusters.py` & `ynab_split_budget-1.0.1/ynabsplitbudget/adjusters.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,16 @@
 class ReconcileAdjuster(Adjuster):
 
 	def filter(self, transactions: List[Transaction]) -> List[Transaction]:
 		return [t for t in transactions if t.cleared == 'cleared']
 
 	def adjust(self, original: Transaction, modifier: Modifier) -> Modifier:
 		modifier.cleared = 'reconciled'
-		modifier.category = self.categories.fetch_by_name('Inflow: Ready to Assign')
+		if not modifier.category:
+			modifier.category = self.categories.fetch_by_name('Inflow: Ready to Assign')
 		return modifier
 
 
 class ClearAdjuster(Adjuster):
 
 	def __init__(self, credentials: Credentials, split_transaction_ids: List[str]):
 		super().__init__(credentials=credentials)
@@ -26,28 +27,29 @@
 	def filter(self, transactions: List[Transaction]) -> List[Transaction]:
 		return [t for t in transactions
 					 	if t.cleared == 'uncleared'
 						and t.id in self.split_transaction_ids]
 
 	def adjust(self, original: Transaction, modifier: Modifier) -> Modifier:
 		modifier.cleared = 'cleared'
-		modifier.category = self.categories.fetch_by_name('Inflow: Ready to Assign')
+		if not modifier.category:
+			modifier.category = self.categories.fetch_by_name('Inflow: Ready to Assign')
 		return modifier
 
 
 class SplitAdjuster(Adjuster):
 
 	def __init__(self, credentials: Credentials, flag_color: str, transfer_payee_id: str, account_id: str):
 		super().__init__(credentials=credentials)
 		self.flag_color = flag_color
 		self.transfer_payee_id = transfer_payee_id
 		self.account_id = account_id
 
 	def filter(self, transactions: List[Transaction]) -> List[Transaction]:
-		return [t for t in transactions if t.cleared == 'cleared' and t.flag_color == self.flag_color
+		return [t for t in transactions if t.cleared == 'cleared' and t.approved and t.flag_color == self.flag_color
 				and not t.subtransactions and not t.account.id == self.account_id]
 
 	def adjust(self, original: Transaction, modifier: Modifier) -> Modifier:
 		split_amount = SplitParser().parse_split(transaction=original)
 		s1 = ModifierSubTransaction(amount=split_amount, payee=self.payees.fetch_by_id(self.transfer_payee_id),
 									memo=f"{original.payee.name} | {original.memo}")
 		s2 = ModifierSubTransaction(amount=original.amount - split_amount, category=original.category, memo=original.memo)
```

### Comparing `ynab_split_budget-1.0.0/ynabsplitbudget/client.py` & `ynab_split_budget-1.0.1/ynabsplitbudget/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,23 +43,24 @@
 		return Account(budget_id=budget_id,
 					   budget_name=budget['name'],
 					   account_id=account_id,
 					   account_name=account['name'],
 					   transfer_payee_id=account['transfer_payee_id'],
 					   currency=budget['currency_format']['iso_code'])
 
-	def fetch_roots(self, since: date) -> List[RootTransaction]:
+	def fetch_roots(self, since: date, include_uncleared: bool) -> List[RootTransaction]:
 		url = f'{YNAB_BASE_URL}budgets/{self.budget_id}/accounts/{self.account_id}/transactions'
 		r = self.session.get(url, params={'since_date': datetime.strftime(since, '%Y-%m-%d')})
 		r.raise_for_status()
 		transactions_dicts = r.json()['data']['transactions']
-		transactions_filtered = [t for t in transactions_dicts if not t['cleared'] == 'uncleared'
-							  and t['deleted'] is False
+		transactions_filtered = [t for t in transactions_dicts if t['deleted'] is False
 							  and (t['import_id'] is None or 's||' not in t['import_id'])
 							  and t['payee_name'] != 'Reconciliation Balance Adjustment']
+		if not include_uncleared:
+			transactions_filtered = [t for t in transactions_filtered  if not t['cleared'] == 'uncleared']
 		transactions = [self.transaction_builder.build_root(t_dict=t) for t in transactions_filtered]
 		return transactions
 
 	def fetch_lookup(self, since: date) -> List[Union[RootTransaction, LookupTransaction, ComplementTransaction]]:
 		url = f'{YNAB_BASE_URL}budgets/{self.budget_id}/transactions'
 		r = self.session.get(url, params={'since_date': datetime.strftime(since, '%Y-%m-%d')})
 		r.raise_for_status()
```

### Comparing `ynab_split_budget-1.0.0/ynabsplitbudget/models/user.py` & `ynab_split_budget-1.0.1/ynabsplitbudget/models/user.py`

 * *Files identical despite different names*

### Comparing `ynab_split_budget-1.0.0/ynabsplitbudget/splitparser.py` & `ynab_split_budget-1.0.1/ynabsplitbudget/splitparser.py`

 * *Files identical despite different names*

### Comparing `ynab_split_budget-1.0.0/ynabsplitbudget/syncrepository.py` & `ynab_split_budget-1.0.1/ynabsplitbudget/syncrepository.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,22 +4,23 @@
 from ynabsplitbudget.client import Client
 from ynabsplitbudget.models.transaction import RootTransaction, ComplementTransaction, LookupTransaction
 from ynabsplitbudget.models.user import User
 
 
 class SyncRepository:
 
-	def __init__(self, user: User, partner: User):
+	def __init__(self, user: User, partner: User, include_uncleared: bool):
 		self._user_client = Client(token=user.token, budget_id=user.budget_id, account_id=user.account_id,
 								   user_name=user.name)
 		self._partner_client = Client(token=partner.token, budget_id=partner.budget_id, account_id=partner.account_id,
 									  user_name=partner.name)
+		self.cleared_only = include_uncleared
 
 	def fetch_roots_wo_complement(self, since: date) -> List[RootTransaction]:
-		roots = self._user_client.fetch_roots(since=since)
+		roots = self._user_client.fetch_roots(since=since, include_uncleared=self.cleared_only)
 		pl = [t for t in self._partner_client.fetch_lookup(since) if isinstance(t, ComplementTransaction)]
 		roots_wo_complement = [t for t in roots if t.share_id not in [lo.share_id for lo in pl]]
 		transactions_replaced_payee = self.replace_payee(transactions=roots_wo_complement,
 															 lookup_date=since)
 		return transactions_replaced_payee
 
 	def insert_complements(self, transactions: List[RootTransaction]) -> List[ComplementTransaction]:
```

### Comparing `ynab_split_budget-1.0.0/ynabsplitbudget/transactionbuilder.py` & `ynab_split_budget-1.0.1/ynabsplitbudget/transactionbuilder.py`

 * *Files identical despite different names*

### Comparing `ynab_split_budget-1.0.0/ynabsplitbudget/ynabsplitbudget.py` & `ynab_split_budget-1.0.1/ynabsplitbudget/ynabsplitbudget.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import logging
 from datetime import date, timedelta, datetime
 from typing import List, Optional
 
 from ynabtransactionadjuster import Credentials, Transaction
 
-from ynabsplitbudget.adjusters import ReconcileAdjuster, SplitAdjuster, ClearAdjuster
+from ynabsplitbudget.adjusters import SplitAdjuster
 from ynabsplitbudget.client import Client
 from ynabsplitbudget.models.exception import BalancesDontMatch
-from ynabsplitbudget.models.transaction import ComplementTransaction, RootTransaction
+from ynabsplitbudget.models.transaction import ComplementTransaction
 from ynabsplitbudget.models.user import User
 from ynabsplitbudget.syncrepository import SyncRepository
 
 
 class YnabSplitBudget:
 	"""Interface to YNAB Split Budget.
 
@@ -20,55 +20,45 @@
 	:ivar logger: Logger of the instance
 	"""
 	def __init__(self, user: User, partner: User):
 		self.user = user
 		self.partner = partner
 		self.logger = self._set_up_logger()
 
-	def push(self, since: date = None) -> List[ComplementTransaction]:
+	def push(self, include_uncleared: bool = False, since: date = None) -> List[ComplementTransaction]:
 		"""Pushes transactions from user split account to partner split account. By default, considers transactions of
 		last 30 days.
 
+		:param include_uncleared: If set to True, will also consider uncleared transactions
 		:param since: If set to date, will push transactions from that date onwards instead of default 30 days
 		:return: List of inserted transactions in partner split account
 		"""
 		since = self._substitute_default_since(since)
-		repo = SyncRepository(user=self.user, partner=self.partner)
+		repo = SyncRepository(user=self.user, partner=self.partner, include_uncleared=include_uncleared)
 		transactions = repo.fetch_roots_wo_complement(since=since)
 
 		complement_transactions = repo.insert_complements(transactions)
 		logging.getLogger(__name__).info(f'inserted {len(complement_transactions)} complements into account of '
 										 f'{self.partner.name}')
 		return complement_transactions
 
-	def split(self, clear: bool = False) -> List[Transaction]:
+	def split(self) -> List[Transaction]:
 		"""Splits transactions (by default 50%) into subtransaction with original category and transfer subtransaction
 		to split account
 
-		:param clear: If set to true transactions in split account will automatically be set to cleared
 		:return: list with split transactions
 		"""
 		creds = Credentials(token=self.user.token, budget=self.user.budget_id)
 		s = SplitAdjuster(creds, flag_color=self.user.flag_color,
 						  transfer_payee_id=self.user.fetch_account().transfer_payee_id,
 						  account_id=self.user.account_id)
 		mod_trans = s.apply()
 		updated_transactions = s.update(mod_trans)
 		logging.getLogger(__name__).info(f'split {len(updated_transactions)} transactions for {self.user.name}')
 
-		if clear:
-			transfer_transaction_ids = [st.transfer_transaction_id for t in updated_transactions for st in
-										t.subtransactions if st.transfer_transaction_id]
-			creds = Credentials(token=self.user.token, budget=self.user.budget_id,
-								account=self.user.account_id)
-			ca = ClearAdjuster(creds, split_transaction_ids=transfer_transaction_ids)
-			mod_trans_clear = ca.apply()
-			count_clear = len(s.update(mod_trans_clear))
-			logging.getLogger(__name__).info(f'cleared {count_clear} transactions for {self.user.name}')
-
 		return updated_transactions
 
 	def raise_on_balances_off(self):
 		"""Evaluates cleared balances in both accounts
 
 		:raises BalancesDontMatch: if cleared amounts in both accounts don't match
 		"""
@@ -90,29 +80,14 @@
 		c = Client(user_name=self.partner.name, budget_id=self.partner.budget_id, account_id=self.partner.account_id,
 				   token=self.partner.token)
 		[c.delete_complement(oc.id) for oc in orphaned_complements]
 		logging.getLogger(__name__).info(f'deleted {len(orphaned_complements)} orphaned complements in account of {self.partner.name}')
 		logging.getLogger(__name__).info(orphaned_complements)
 		return orphaned_complements
 
-	def reconcile(self) -> int:
-		"""Reconciles cleared transactions in the current account
-
-		:returns: count of reconciled transactions
-		:raises BalancesDontMatch: if cleared amounts in both accounts don't match
-		"""
-		self.raise_on_balances_off()
-		creds = Credentials(token=self.user.token, budget=self.user.budget_id,
-							account=self.user.account_id)
-		ra = ReconcileAdjuster(creds)
-		mod_trans = ra.apply()
-		updated_trans = ra.update(mod_trans)
-		logging.getLogger(__name__).info(f'reconciled {len(updated_trans)} transactions for {self.user.name}')
-		return len(updated_trans)
-
 	@staticmethod
 	def _substitute_default_since(since: Optional[date]) -> date:
 		if since is None:
 			return datetime.now() - timedelta(days=30)
 		return since
 
 	@staticmethod
```

### Comparing `ynab_split_budget-1.0.0/PKG-INFO` & `ynab_split_budget-1.0.1/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,28 +1,7 @@
-Metadata-Version: 2.1
-Name: ynab-split-budget
-Version: 1.0.0
-Summary: Library to split and share You Need A Budget (YNAB) transactions between two budgets
-License: MIT
-Author: Daniel Basta
-Author-email: ynab@basta.info
-Requires-Python: >=3.8,<4.0
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: pyyaml (>=6.0,<7.0)
-Requires-Dist: requests (>=2.28,<3.0)
-Requires-Dist: ynab-transaction-adjuster (>=2.0.0,<3.0.0)
-Description-Content-Type: text/markdown
-
 # ynab-split-budget
 
 [![GitHub Release](https://img.shields.io/github/release/dnbasta/ynab-split-budget?style=flat)]() 
 [![Github Release](https://img.shields.io/maintenance/yes/2100)]()
 [![Monthly downloads](https://img.shields.io/pypi/dm/ynab-split-budget)]()
 
 This library enables cost sharing across two YNAB budgets. It requires two dedicated accounts in each budget to which
@@ -65,27 +44,32 @@
                account_id='<account_id', flag_color='<flag_color>')
 
 split_budget = YnabSplitBudget(user=user, partner=partner)
 ```
 ### 3. Split transactions
 Call the `split()` method of the instance. It will split flagged transactions in the budget into a subtransaction with
 the original category and a transfer to the split account. By default, the transfer transactions will show up as 
-uncleared in the split account. The optional `clear` parameter allows to automatically clear the transactions in 
-the split account. The function returns the updated transactions after applying the split.
+uncleared in the split account.
 ```py
 split_budget.split()
 ```
 
 ### 4. Push new splits to partner split account
 Calling the `push()` function will insert new transactions from user split account into split account of partner to keep
-both accounts in sync. By default, the function will compare and insert transactions of the last 30 days. Optionally it 
+both accounts in sync. By default, the function will only consider cleared transactions. This is in general a safer 
+option as it forces users to manually check and clear transactions in the split account. However, it makes running the 
+whole functionality automatically cumbersome, hence the function takes an optional `include_uncleared` parameter which, 
+if set to `True`, makes it also consider uncleared transactions. 
+Additionally by default, the function will compare and insert transactions of the last 30 days. Optionally it 
 takes a `since` parameter in the form of `datetime.date` to set a timeframe different from 30 days. 
 
 ```py
 split_budget.push()
+# or optionally with considering uncleared transactions as well
+split_budget.push(include_uncleared=True)
 ```
 ## Advanced Usage
 ### Check Balances
 The `raise_on_balances_off()` function compares the cleared balances in both split accounts. If they don't match it 
 will raise a `BalancesDontMatch` error which includes the values of the balances.
 ```py
 split_budget.raise_on_balances_off()
@@ -94,20 +78,14 @@
 The `delete_orphans()` function deletes orphaned transactions in the partner split account, which don't have a 
 corresponding transaction in the user split account any more. It does return a list with the deleted transactions. 
 By default, the function compares transactions of the last 30 days. Optionally it takes a `since` parameter in the 
 form of `datetime.date` to set a timeframe different from 30 days.
 ```py
 split_budget.delete_orphans()
 ```
-### Reconcile split account
-The `reconcile()` function allows to reconcile the split account. It does check if the balances match before reconciling
-and will an `BalancesDontMatch` error if they don't.
-```py 
-split_budget.reconcile()
-```
 
 ### Show Logs
 The library logs information about the result of the methods at the 'INFO' level. The logs can be made visible by 
 importing the logging module and set it to the level `INFO`. The logger itself can also be accessed via the `logger` 
 attribute of the instance.
 ```py
 import logging
@@ -119,8 +97,7 @@
 ```bash
 $ python -m ynabsplitbudget -u <path/user.yaml> -p <path/partner.yaml> --split
 ```
 For a complete list of available bash options please use
 ```bash
 $ python -m ynabsplitbudget -h | -- help
 ```
-
```

